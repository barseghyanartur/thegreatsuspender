# Tab Suspender

<img src="/src/img/suspendy-guy.png" width="100px" />

"Tab Suspender" is a free and open-source Google Chrome extension for people who find that chrome is consuming too much system resource or suffer from frequent chrome crashing. Once installed and enabled, this extension will automatically *suspend* tabs that have not been used for a while, freeing up memory and cpu that the tab was consuming.

If you have suggestions or problems using the extension, please [submit a bug or a feature request](https://github.com/barseghyanartur/tabsuspender/issues/). For other enquiries you can email me at artur.barseghyan@gmail.com.

**If you have lost tabs from your browser:** I have written a guide for how to recover your lost tabs [here](https://github.com/barseghyanartur/tabsuspender/issues/526
).

### Credits

This is a fork of once famous The Great Suspender extension for Chromium based 
browsers.

Current master represents a slightly changed version of the v7.1.6 (tag) of
the original package. All changes are listed in the CHANGELOG.md.

Originally created by [Dean Oemcke](https://github.com/deanoemcke).

### Chrome Web Store

Tab Suspender is [available via the official Chrome Web Store](https://chrome.google.com/webstore/detail/tab-suspender/klbibkeccnjlkjkiokjodocebajanakg).

Please note that the webstore version may be behind the latest version here. That is because I try to keep webstore updates down to a minimum due to their [disruptive effect](https://github.com/barseghyanartur/tabsuspender/issues/526).

For more information on the permissions required for the extension, please refer to this gitHub issue: (https://github.com/barseghyanartur/tabsuspender/issues/213)

### Install as an extension from source

1. Download the **[latest available version](https://github.com/barseghyanartur/tabsuspender/releases)** and unarchive to your preferred location (whichever suits you).
2. Using **Google Chrome** browser, navigate to chrome://extensions/ and enable "Developer mode" in the upper right corner.
3. Click on the <kbd>Load unpacked extension...</kbd> button.
4. Browse to the src directory of the unarchived folder and confirm.

If you have completed the above steps, the "welcome" page will open indicating successful installation of the extension.

Be sure to unsuspend all suspended tabs before removing any other version of the extension or they will disappear forever!

### Build from github

Dependencies: openssl, npm.

Clone the repository and run these commands:
```
npm install
npm run generate-key
npm run build
```

It should say:
```
Done, without errors.
```

The extension in crx format will be inside the build/crx/ directory. You can drag it into [extensions] (chrome://extensions) to install locally.

### Integrating with another Chrome extension or app

This extension has a small external api to allow other extensions to request the suspension of a tab. See [this issue](https://github.com/barseghyanartur/tabsuspender/issues/276) for more information. And please let me know about it so that I can try it out!

### Contributing to this extension

Contributions are very welcome. Feel free to submit pull requests for new features and bug fixes. For new features, ideally you would raise an issue for the proposed change first so that we can discuss ideas. This will go a long way to ensuring your pull request is accepted.

### License

This work is licensed under a GNU GENERAL PUBLIC LICENSE (v2)

### Shoutouts

This package uses the [html2canvas](https://github.com/niklasvh/html2canvas) library written by Niklas von Hertzen.  
It also uses the indexedDb wrapper [db.js](https://github.com/aaronpowell/db.js) written by Aaron Powell.  
Thank you also to [BrowserStack](https://www.browserstack.com) for providing free chrome testing tools.
