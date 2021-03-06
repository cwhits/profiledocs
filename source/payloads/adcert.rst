.. _payloadtype-com.apple.ADCertificate.managed:

Active Directory Certificate
============================
:download:`Template <../_static/examples/com.apple.ADCertificate.managed.mobileconfig>`

You can request a certificate from a Microsoft Certificate Authority (CA) using DCE/RPC and the
Active Directory Certificate profile payload instructions detailed at https://support.apple.com/kb/HT5357.

.. contents::

Summary
-------

.. pfmheader:: /_static/manifests/com.apple.ADCertificate.managed manifest.plist

Keys
----

.. pfmkey:: Description /_static/manifests/com.apple.ADCertificate.managed manifest.plist
.. pfmkey:: CertServer /_static/manifests/com.apple.ADCertificate.managed manifest.plist
.. pfmkey:: CertTemplate /_static/manifests/com.apple.ADCertificate.managed manifest.plist
.. pfmkey:: CertificateAuthority /_static/manifests/com.apple.ADCertificate.managed manifest.plist
.. pfmkey:: CertificateAcquisitionMechanism /_static/manifests/com.apple.ADCertificate.managed manifest.plist
.. pfmkey:: CertificateRenewalTimeInterval /_static/manifests/com.apple.ADCertificate.managed manifest.plist
.. pfmkey:: Keysize /_static/manifests/com.apple.ADCertificate.managed manifest.plist
.. pfmkey:: UserName /_static/manifests/com.apple.ADCertificate.managed manifest.plist
.. pfmkey:: Password /_static/manifests/com.apple.ADCertificate.managed manifest.plist
.. pfmkey:: PromptForCredentials /_static/manifests/com.apple.ADCertificate.managed manifest.plist

.. warning:: PromptForCredentials seems to have no effect on manually installed profiles. They still ask for credentials.

.. pfmkey:: AllowAllAppsAccess /_static/manifests/com.apple.ADCertificate.managed manifest.plist

Links
-----

- `macmules blog: OSX & AD CERTIFICATE REQUESTS, SOME TIPS <https://macmule.com/2015/09/06/osx-ad-certificate-requests-some-tips/>`_.
- `Certificate Renewal Behaviour <https://support.apple.com/en-us/HT204446>`_.

Troubleshooting
---------------

.. warning:: As of approx 10.12.4 you can no longer select a transport. And you will not be able to install the payload
    if the client is not bound to a directory.

- If you request a `User` certificate but the payload is in the `System` PayloadScope, the User certificate will be requested as the
  computer account. Normally the certificate policy will deny this, so check that you have the correct scope.

Uninstall Behaviour
-------------------

- The certificate is not revoked upon uninstallation.
- The certificate is not removed from keychain, but the private key IS removed. The private key is named after the issuing host.


