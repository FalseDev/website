---
title: "Vanilla OS 2.0 Orchid - Initial Work"
description: "We started the development of Vanilla OS 2.0 Orchid."
published: 2023-03-02
layout: article
published: false
comments: true
---

We are happy to announce the start of development for the second version of Vanilla OS. The new version will be called **2.0 Orchid** and will be released independently of Ubuntu's release schedule.

## New Versioning

One of the most significant changes in Vanilla OS 2.0 Orchid will be its base on **Ubuntu 23.04 Lunar**. However, we have decided to abandon the codenames and versioning of Ubuntu to give Vanilla OS more freedom in releases and to reduce pressure on development.

In doing so, we are also distancing ourselves from Canonical's choices, which are pushing for the adoption of Snap at the expense of user experience, at least from our point of view. We want to maintain the choice for users to use Snap or traditional packages, and we do not want packages in the Ubuntu repo to be modified to push Snap usage, as is happening with [Firefox](https://packages.ubuntu.com/kinetic/firefox) and other packages. We have received many reports from users who installed Firefox and other packages via Apx, only to find Snap installed because of those transitional packages.

## The Codename

Vanilla includes about 110 species of orchids, the most famous of which is the flat vanilla (V. planifolia), native to Mexico and Belize, from which the flavor of vanilla used in food, cosmetics, and perfumery is extracted.

The choice of Orchid as the name for the new version of Vanilla OS was inspired by the beauty and grace of orchids, especially the Vanilla genus. Like the plant from which it takes its name, Vanilla OS 2.0 Orchid is destined to bring a new fragrance to the Linux world, offering a more reliable and consistent user experience in every aspect.

## OEM Support

We are also working to allow the sale of devices with pre-installed Vanilla OS, and for this reason we are focusing on the OEM (Original equipment manufacturer) part.

We are adapting the installer and first setup to allow the user to configure their account and preferences after the installation phase, thus allowing pre-installation of the operating system without requiring the creation of a user, which is useful when providing a device with pre-installed Vanilla OS or when installing it for friends, relatives, and colleagues who may not be able to perform the installation process on their own.

One of the main changes to the First Setup will be the presence of two new modes: Express and Advanced. The user will be able to choose whether to proceed with our pre-set settings or autonomously, deciding on the package format, whether to install proprietary drivers and codecs, and more.

## GNOME 44

We intend to distribute GNOME 44 in the next version of Vanilla OS, but this may depend on any slowdowns in the release by GNOME or the packaging of some libraries by Ubuntu. We will then evaluate whether it will be possible to package GNOME 44 on our own if necessary.

## Kernel 6+

The kernel will be updated to a version equal to or higher than 6. We will decide after April 6, 2023, Ubuntu's kernel freeze, whether to use the kernel provided by Ubuntu or whether it will be necessary to update it ourselves, in order to ensure compatibility with the latest devices and peripherals.

Among other things, there will be the usual updates to Apx, Vso, and ABRoot to resolve bugs reported during the development phase, as well as the update of the necessary libraries for their operation.

## Plans for the Future

Looking to the future, we have several ambitious plans to further improve Vanilla OS.

## Debian Rebase

One of the main goals is to migrate to a Debian base, completely eliminating Ubuntu as an intermediary. This is due to the increasing presence of altered packages in Ubuntu, which often require patch cleanup to provide a stock version of the software. Testing for this migration is already underway using the unstable branch of Debian, and the results so far are very promising.

The unstable branch is known to receive updates very frequently, which is why we will manage an internal freeze to ensure greater security and stability.

## ABRoot OCI Support

Another important project is the introduction of OCI support in ABRoot. With the use of images in ABRoot, we will have greater control over the release of updates as well as more time to test them before release. The new update system will therefore take care of downloading and extracting the update, avoiding the use of the package manager and ensuring an exact copy of the system, while still maintaining the changes imposed by the user.

This change was originally planned for version 2.0 of Vanilla OS, but due to the significant changes it will bring to the operating system's structure, it has been decided to postpone it until the migration to Debian.