# node-libuuid

## Description
A node C binding to the libuuid library's uuid_generate().
NOTE: The uuid returned is lowercased.

## Prerequisites
You must have libuuid installed on your machine.
In Ubuntu:
    apt-get install uuid-dev

## Install
    npm install libuuid

## Usage
    var libuuid = require('libuuid');
    var uuid_val = libuuid.create();
    console.log(" UUID = ", uuid_val);

    // If you want to use libuuid as a drop in replacement for node-uuid then simply do
    var uuid = require('libuuid').create;
    var uuid_val = uuid();
    console.log(" UUID = ", uuid_val);

