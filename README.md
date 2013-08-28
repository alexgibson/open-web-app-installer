Open Web Installer
==================

A custom UI component for installing [Open Web Apps](https://developer.mozilla.org/en-US/docs/Web/Apps) on Firefox OS, Firefox for Android and Firefox for desktop.

This project is still in beta status

Installation
---------------------------------------

* Download: [zip](https://github.com/alexgibson/open-web-installer/archive/master.zip)
* Git: `git clone https://github.com/alexgibson/open-web-installer.git`

Setup
---------

This component can be used as an AMD module, or a global.

To use create a new `Installer` instance, passing the relevant callbacks you need.

```
var page = new Installer({
    onSuccess: successCallback,
    onError: errorCallback
});

function successCallback () {
    console.log('Installer() success');
}

function errorCallback (error) {
    console.error('Installer() error: ' + error);
}
```
