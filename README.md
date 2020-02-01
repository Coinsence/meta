# Coinsence ![GitHub](https://img.shields.io/github/license/Coinsence/coinsence-monorepo.svg)

This is meta product development repository.


# Table of content

- **[Introduction](#introduction)**
- **[Repositories](#repositories)**
- **[Development](#development)**
	- **[Cloning project](#cloning-project)**
	- **[Running locally](#running-locally)**
	- **[Installing modules](#installing-modules)**
	- **[Testing](#testing)**
- **[Open source community](#open-source-community)**
	- **[Issues](#issues)**
	- **[Contributing](#contributing)**


# Introduction

Coinsence is a collaboration platform that allows communities to issue their own tokens to mobilize people, engage resources and reward contributions.

To test the current solution, everybody is welcome to join the network via their email adress under www.coinsence.org

Basically, HumHub - Open Source Social Network is enhanced with further modules enabling: 
- spaces (communities, projects, organizations) to issue their own space coins. 
- spaces to create internal accounts which can be managed by different users.
- user to create own accounts.
- user to perform transactions of coins between different accounts.
- spaces can create tasks and allocate specifoc coins to the tasks.
- spaces to collect coins via. crowd-funding. 
- User and spaces to share resources, goods, products and services in a common marketplace. 

To ensure data integrity and interoperability, Coinsence uses Ethereum as decentral common ledger to store and exchange token (coins). 

An independent android mobile application for transactions is also deployed in the playstore under coinsence. 

**What is the benefits of using coins?**
Space_Y can distributes during crowd-funding process space_y_coins to crowd-investors and can also distribute space_y_coins to other contributors. With space_y_coins, space_y can show the contribution of other spaces and users to space_y. The coins which are a proof-of-contribution can be used later to track voluntary contributions or as proof-of-investment to map later equity and revenue share to the different contributing members and groups.

**What is the benefit of crowd-fund?**
Crowdfunding enables spaces to exchange coins as instrument to share value. Further more, crowd-funding enables community members to decide collectively over investment and project support e.g. which projects shall receive community coins (User can allocate space_y_coins to space_x and get in exchange space_x_coins).
Via crowd-funding, projects (e.g. space_x) can get community coins (e.g. space_y_coins) which they can use to get resources from the marketplace which are requesting space_y_coins. In counterpart, space_y has space_x_coins.

**What is the benefit of the marketplace?**
Communities can share resources via. the marketplace. User making offers in the marketplace can set the price in a specific space coins as exchange unit or can set the discount they offer in exchange of specific space coins.


# Repositories

##### [humhub](https://github.com/Coinsence/humhub):

HumHub fork as basis for the social network.

##### [humhub-modules-xcoin ](https://github.com/Coinsence/humhub-modules-xcoin):

Module enabling coin creation and exchange.

##### [humhub-modules-ethereum](https://github.com/Coinsence/humhub-modules-ethereum):

Smart contracts integration with humhub-modules-xcoin.

##### [coinsence-monorepo](https://github.com/Coinsence/coinsence-monorepo):

Smart contracts used for coinsence project.

##### [coinsence-wallet](https://github.com/Coinsence/coinsence-wallet):

Coinsence ERC20 mobile wallet.

##### [coinsence-docker](https://github.com/Coinsence/coinsence-docker):

A coinsence docker implementation.


# Development

So below are the main steps in order to get Coinsence project started & running.

Before starting, you can choose whether you should work using [docker](https://github.com/Coinsence/coinsence-docker) to automate some configurations or do all of that manually, either ways you should get the same results.


### Cloning project

First thing first, start by cloning the humhub repo locally.

	git clone https://github.com/Coinsence/humhub

Alternatievely, you can also fork it first to your git, and clone the forked repo locally.

	git clone https://github.com/username/humhub

### Running locally

To install humhub locally, make sure first that you have the proper dev environment, to do so check the official humhub [documentation](http://docs.humhub.org/admin-requirements.html).

Once you've met all the requirements, move on to the installation process following the official [guide](http://docs.humhub.org/admin-installation.html).

Finally, you can finish off the installation with some basic configurations using -you guessed it- the official [guide](http://docs.humhub.org/admin-installation-configuration.html).

### Installing modules

Installing modules can be done using two ways, either automatically through *Browse online* tab in the *Administration menu* or manually by placing it under a know path, this latter can be configured using this small code block in the `protected/config/common.php` file (see also [docs](http://docs.humhub.org/dev-environment.html#external-modules-directory)):

	return [
        'params' => [
            'moduleAutoloadPaths' => ['/some/folder/modules'],        
        ],
    ]

To check if module is installed or detected by humhub, click on Modules in the *Administration menu*, if the installation is successful, you'll see your installed module, to start using it, just click `Enable` and there you have it.


### Testing

Humhub comes prebundled with codeception framework for testing, you can check some of the implemented tests in `tests` folder under the root of the built-in/custom modules.

Just follow along those tests and start rocking some tests.

Some modules (xcoin & ethereum) comes pre-configured with travis-ci and coveralls, so don't bother with that if you're developing some tests for those modules.

Also [here](http://docs.humhub.org/dev-testing.html)'s the official documentation used to develop some of the test suites.



# Open source community

As a open source community, we are always open to discussions and changes, for more info please check out code of conduct [document](https://github.com/Coinsence/meta/blob/master/CODE_OF_CONDUCT.md).

### Issues

We keep track of project global [issues](https://github.com/Coinsence/meta/issues) in a separate repository named `meta`, along with repositories issues.

If you come across an issue with any of the aformentioned repos, do a search in the Issues tab of that repo to make sure it hasn't been reported before. Follow these steps to help us prevent duplicate issues and unnecessary notifications going to the many people watching this repo:

- If the issue you found has been reported and is still open, and the details match your issue, give a "thumbs up" to the relevant posts in the issue thread to signal that you have the same issue. No further action is required on your part.
- If the issue you found has been reported and is still open, but the issue is missing some details, you can add a comment to the issue thread describing the additional details.
- If the issue you found has been reported but has been closed, you can comment on the closed issue thread and ask to have the issue reopened because you are still experiencing the issue. Alternatively, you can open a new issue, reference the closed issue by number or link, and state that you are still experiencing the issue. Provide any additional details in your post so we can better understand the issue and how to fix it.

### Contributing

In order to contribute to the coinsence project, please fork the targeted repository and make a PR.

Thanks for taking time reading this wonderful document.

Written with Love & Pain.

