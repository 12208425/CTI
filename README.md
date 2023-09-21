# CTI
{
    "version": "1.0",
    "format_version": "1.0",
    "update_date": "2023-04-21T11:43Z",
    "dictionary": [
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "Microsoft Corporation"
                ],
                "product": [
                    "^Microsoft ASP.NET Core ([0-9]\\.*[0-9]*\\.*[0-9]*)"
                ],
                "version": [
                    "^Microsoft ASP.NET Core ([0-9]\\.*[0-9]*\\.*[0-9]*)"
                ]
            },
            "translation": {
                "vendor": [
                    "microsoft"
                ],
                "product": [
                    "asp.net_core"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "set_version_if_product_matches",
                "replace_product"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "Microsoft Corporation"
                ],
                "product": [
                    "Microsoft Edge"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "microsoft"
                ],
                "product": [
                    "edge_chromium"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "www\\.wireshark\\.org"
                ],
                "product": [
                    "Wireshark"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "wireshark"
                ],
                "product": [
                    "wireshark"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^Oracle",
                    "^Sun"
                ],
                "product": [
                    "Java.* Development Kit",
                    "^Oracle.*VirtualBox [0-9]+",
                    "^Java.*Update"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "oracle",
                    "sun"
                ],
                "product": [
                    "jdk",
                    "vm_virtualbox",
                    "jre"
                ],
                "version": []
            },
            "action": [
                "replace_vendor_if_matches",
                "replace_product_if_matches"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^Microsoft Corporation"
                ],
                "product": [
                    "^Microsoft Office"
                ],
                "version": [
                    "^Microsoft Office.*([0-9]{4})"
                ]
            },
            "translation": {
                "vendor": [
                    "microsoft"
                ],
                "product": [
                    "office"
                ],
                "version": [],
                "msu_name": [
                    "Microsoft Office $(VERSION)"
                ]
            },
            "action": [
                "replace_vendor",
                "replace_product",
                "set_version_only_if_product_matches",
                "replace_msu_name",
                "check_hotfix"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^Mozilla"
                ],
                "product": [
                    "^Mozilla Firefox ([0-9]+\\.*[0-9]*\\.*[0-9]* )*ESR",
                    "^Mozilla Firefox",
                    "^Mozilla Thunderbird",
                    "^SeaMonkey"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "mozilla"
                ],
                "product": [
                    "firefox_esr",
                    "firefox",
                    "thunderbird",
                    "seamonkey"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product_if_matches"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^Google"
                ],
                "product": [
                    "^Google Update Helper",
                    "^Google Chrome"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "google"
                ],
                "product": [
                    "update_helper",
                    "chrome"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product_if_matches"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^Adobe"
                ],
                "product": [
                    "^Adobe Flash Player",
                    "^Adobe Shockwave Player",
                    "^Adobe Reader",
                    "^Adobe Acrobat Reader DC",
                    "^Adobe AIR"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "adobe"
                ],
                "product": [
                    "flash_player",
                    "shockwave_player",
                    "acrobat_reader",
                    "acrobat_reader_dc",
                    "adobe_air"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product_if_matches"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^Opera Software"
                ],
                "product": [
                    "^Opera Stable"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "opera"
                ],
                "product": [
                    "opera_browser"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^Skype",
                    "^Microsoft"
                ],
                "product": [
                    "^Skype for Business",
                    "^Skype"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "skype",
                    "microsoft"
                ],
                "product": [
                    "skype_for_business",
                    "skype"
                ],
                "version": []
            },
            "action": [
                "replace_vendor_if_matches",
                "replace_product_if_matches"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^Apple"
                ],
                "product": [
                    "^Safari",
                    "^iTunes",
                    "^QuickTime"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "apple"
                ],
                "product": [
                    "safari",
                    "itunes",
                    "quicktime"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product_if_matches"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^VMware"
                ],
                "product": [
                    "^VMware Workstation$",
                    "^VMware Player$",
                    "test_entry"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "vmware"
                ],
                "product": [
                    [
                        "workstation",
                        "workstation_pro (version >= 12.0.0)"
                    ],
                    [
                        "workstation_player (version >= 12.0.0)",
                        "workstation (version >= 12.0.0)",
                        "player (version < 12.0.0)"
                    ],
                    "test_entry_translation"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product_if_matches"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^RealNetworks"
                ],
                "product": [
                    "^RealPlayer"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "realnetworks"
                ],
                "product": [
                    "realplayer"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^Oracle",
                    "^MySQL"
                ],
                "product": [
                    "^MySQL Server"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "oracle",
                    "mysql"
                ],
                "product": [
                    "mysql"
                ],
                "version": []
            },
            "action": [
                "replace_vendor_if_matches",
                "replace_product"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^ImageMagick"
                ],
                "product": [
                    "^ImageMagick"
                ],
                "version": [
                    "^ImageMagick ([0-9]+\\.*[0-9]*\\.*[0-9]*-*[0-9]*)"
                ]
            },
            "translation": {
                "vendor": [
                    "imagemagick"
                ],
                "product": [
                    "imagemagick"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product",
                "set_version_if_product_matches"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [],
                "product": [
                    "^QEMU"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "qemu"
                ],
                "product": [
                    "qemu"
                ],
                "version": []
            },
            "action": [
                "replace_product"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^PostgreSQL"
                ],
                "product": [
                    "^PostgreSQL ([0-9]+\\.*[0-9]*\\.*[0-9]*)"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "postgresql"
                ],
                "product": [
                    "postgresql"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^VideoLAN"
                ],
                "product": [
                    "^VLC media player"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "videolan"
                ],
                "product": [
                    "vlc_media_player"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [],
                "product": [
                    "^Pidgin"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "pidgin"
                ],
                "product": [
                    "pidgin"
                ],
                "version": []
            },
            "action": [
                "replace_product"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^Cisco Systems"
                ],
                "product": [
                    "^ClamAV"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "clamav"
                ],
                "product": [
                    "clamav"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^Hewlett Packard"
                ],
                "product": [
                    "^HPE System Management Homepage"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "hp"
                ],
                "product": [
                    "system_management_homepage"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^Jenkins"
                ],
                "product": [
                    "^Jenkins"
                ],
                "version": [
                    "^Jenkins ([0-9]+\\.*[0-9]*\\.*[0-9]*)"
                ]
            },
            "translation": {
                "vendor": [
                    "jenkins"
                ],
                "product": [
                    "jenkins"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product",
                "set_version_if_product_matches"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^Python"
                ],
                "product": [
                    "^Python [0-9]\\.[0-9]+\\.*[0-9]* \\("
                ],
                "version": [
                    "^Python ([0-9]\\.[0-9]+\\.[0-9])"
		],
                "target_hw" : [
                    "^Python [0-9]+\\.*[0-9]*\\.*[0-9]* \\(([6432]{2}-bit)\\)"
                ]
            },
            "translation": {
                "vendor": [
                    "python"
                ],
                "product": [
                    "python"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product",
		"set_version_if_product_matches",
                "set_targethw_if_product_matches"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^Microsoft Corporation"
                ],
                "product": [
                    "^Microsoft Exchange Server"
                ],
                "version": [
                    "^Microsoft Exchange Server ([0-9]{4})"
                ],
                "update":[
                    "^Microsoft Exchange Server.*Update ([0-9]+)"
                ]
            },
            "translation": {
                "vendor": [
                    "microsoft"
                ],
                "product": [
                    "exchange_server"
                ],
                "version": [],
                "update":[
                    "cumulative_update_$(UPDATE)"
                ],
                "msu_name": [
                    "Microsoft Exchange Server $(VERSION) Cumulative Update $(UPDATE)"
                ]
            },
            "action": [
                "replace_vendor",
                "replace_product",
                "set_version_if_product_matches",
                "set_update_if_product_matches",
                "replace_msu_name",
                "check_hotfix"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^Wazuh.*"
                ],
                "product": [
                    "^Wazuh Agent"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "wazuh"
                ],
                "product": [
                    "wazuh"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product"
            ]
        },
        {
            "target": "windows",
            "source": {
                "vendor": [
                    "^The Apache Software"
                ],
                "product": [
                    "^Apache Tomcat.*"
                ],
                "version": []
            },
            "translation": {
                "vendor": [
                    "apache"
                ],
                "product": [
                    "tomcat"
                ],
                "version": []
            },
            "action": [
                "replace_vendor",
                "replace_product"
            ]
        }
    ],
    "license": {
        "title": "Dictionary of CPEs to analyze system vulnerabilities.",
        "copyright": "Copyright (C) 2015, Wazuh Inc.",
        "date": "March 6, 2019.",
        "type" : "GPLv2"
    }
}
