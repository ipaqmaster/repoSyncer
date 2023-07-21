# repoSyncer

## About

This is a script made to help me sync RPM repositories autonomously for serving local clients. A wrapper for `reposync` from yum-utils which takes any filename.repo and processes it for enabled repos to copy locally.

## Usage

Run `main /etc/yum.repos.d/rocky.repo` for example and it will look for enabled repos and sync them locally. Currently this is hardcoded to /repo/upstream however that may change in a future push.

I've been using this in conjunction with the sister project [isoManager](https://github.com/ipaqmaster/isoManager) for the automated provisioning of RedHat-based hosts and the tiered management of their updates..

## What's supported / tested?

This script was written for RHEL-based systems such a Rocky 9 and should work on any of them (Or any other distro where `reposync` and `dnf` are intentionally made avaiable.)
