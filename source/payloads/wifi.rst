.. _payloadtype-com.apple.wifi.managed:

Wi-Fi
=====

.. warning:: The profile cannot be installed if your machine does not have a Wi-Fi AirPort adapter. USB Adapters do not
    qualify, so you may have issues testing in a Virtual Machine. This is because it uses CoreWLAN to make the settings
    and CoreWLAN will only return AirPort devices.

.. contents::

Summary
-------

.. pfmheader:: /_static/manifests/com.apple.wifi.managed manifest.plist

Keys
----

.. pfmkey:: SSID_STR /_static/manifests/com.apple.wifi.managed manifest.plist

- In iOS 7.0 and later, this is optional if a DomainName value is provided

.. pfmkey:: HIDDEN_NETWORK /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: AutoJoin /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: CaptiveBypass /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: EncryptionType /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: Password /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: PayloadCertificateUUID /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: TLSCertificateRequired /_static/manifests/com.apple.wifi.managed manifest.plist

Keys (HotSpot)
--------------

.. pfmkey:: IsHotspot /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: DomainName /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: DisplayedOperatorName /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: ServiceProviderRoamingEnabled /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: RoamingConsortiumOIs /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: NAIRealmNames /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: MCCAndMNCs /_static/manifests/com.apple.wifi.managed manifest.plist

Keys (802.1x)
-------------

.. pfmkey:: EAPClientConfiguration /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfm:: /_static/manifests/com.apple.wifi.managed manifest.plist
    :key: EAPClientConfiguration

.. pfmkey:: EAPClientConfiguration:AcceptEAPTypes /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: EAPClientConfiguration:UserName /_static/manifests/com.apple.wifi.managed manifest.plist


.. pfmkey:: EAPClientConfiguration:UserPassword /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: EAPClientConfiguration:OneTimeUserPassword /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: EAPClientConfiguration:PayloadCertificateAnchorUUID /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: EAPClientConfiguration:TLSTrustedServerNames /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: EAPClientConfiguration:TLSAllowTrustExceptions /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: EAPClientConfiguration:TTLSInnerAuthentication /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: EAPClientConfiguration:OuterIdentity /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: EAPClientConfiguration:SystemModeCredentialsSource /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: EAPClientConfiguration:EAPFASTUsePAC /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: EAPClientConfiguration:EAPFASTProvisionPAC /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: EAPClientConfiguration:EAPFASTProvisionPACAnonymously /_static/manifests/com.apple.wifi.managed manifest.plist

Keys (Proxy)
------------

.. pfmkey:: ProxyType /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: ProxyServer /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: ProxyUsername /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: ProxyServerPort /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: ProxyPassword /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: ProxyPACURL /_static/manifests/com.apple.wifi.managed manifest.plist
.. pfmkey:: ProxyPACFallbackAllowed /_static/manifests/com.apple.wifi.managed manifest.plist

Keys (QoS)
----------

.. pfmkey:: QoSMarkingPolicy /_static/manifests/com.apple.wifi.managed manifest.plist

Available in iOS 10.0 and later. Not supported in macOS.

Links
-----

- `Official Documentation <https://developer.apple.com/library/content/featuredarticles/iPhoneConfigurationProfileRef/Introduction/Introduction.html#//apple_ref/doc/uid/TP40010206-CH1-SW30>`_.
