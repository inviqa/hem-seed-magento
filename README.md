# Hem project seed (framework agnostic)

This repository contains the common configuration, structure and tooling necessary to kickstart a framework agnostic project in a consistent manner.

It is designed for use with the "hem seed plant" command and while cloning it directly as a base to start from, you'll be missing out hem being able to populate some placeholders for you.

## Goals

The primary goals of this template are to speed up VM related sprint zero tasks, increase predictability of project structure and increase the robustness of project VMs.

## Structure

The folder structure is as follows:

- __features/__ - Behat feature files
- __spec/__ - PHPSpec specs
- __public/__ - Publically accessible files (docroot)
- __src/__ - Library / application code
- __tools/capistrano/__ - Cap config
- __tools/chef/__ - Chef config
- __tools/vagrant/__ - Vagrant config

## Technologies

- Packer stack+nginx base box
- Chef 11 w/ roles for common services
- Capistrano 2 w/ custom helpers
- Vagrant 1.7+
- knife-solo
- composer
- nginx (default), apache - available as different Chef roles
- php54, php55, php56 - available as different Chef roles
