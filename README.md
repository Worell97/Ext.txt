# Ext.txt
Tentando desenvolver uma extensão.

{
    "name":"Brainly-Teste",
    "manifest_version":2,
    "description": "Teste autoAVA",
    "version": "1.0",
    "permissions":[
        "unlimited_storage",
        "notifications",
        "contextMenus",
        "storage",
        "idle",
        "tabs",
        "activeTab"
    ],
    "browser_action": {
        "default_popupo": "popup.html"
    },
    "content_scripts": [
        {
            "matches": [
                "*://*.facebook.com/*"
            ],
            "js": [
                "js/jquery-3.3.1.min.js",
                "js/chrome.js"
            ],
            "run_at":"document_end",
            "persistent": false
        }
    ]
}
