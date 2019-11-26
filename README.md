Dekalee PubSub swarrot
=====================

[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/dekalee/pubsub-swarrot-bundle/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/dekalee/pubsub-swarrot-bundle/?branch=master)
[![Latest Stable Version](https://poser.pugx.org/dekalee/pubsub-swarrot-bundle/v/stable)](https://packagist.org/packages/dekalee/pubsub-swarrot-bundle)
[![Total Downloads](https://poser.pugx.org/dekalee/pubsub-swarrot-bundle/downloads)](https://packagist.org/packages/dekalee/pubsub-swarrot-bundle)
[![License](https://poser.pugx.org/dekalee/pubsub-swarrot-bundle/license)](https://packagist.org/packages/dekalee/pubsub-swarrot-bundle)

This bundle will wrap the [swarrot-pubsub](https://github.com/dekalee/pubsub-swarrot) library.

It will provide a way to use the pubsub provider while using the [SwarrotBundle](https://github.com/swarrot/SwarrotBundle).

Installation
------------

Use composer to install this bundle :

```
    composer require dekalee/pubsub-swarrot-bundle
```

Activate it in the `AppKernel.php` file:

```php
    new Dekalee\PubSubSwarrotBundle\DekaleePubSubSwarrotBundle(),
```

Configuration
-------------

In your `config.yml` file, you should set the provider to pubsub and specify the connection :

```yaml
    swarrot:
        provider: pub_sub
        default_connection: pub_sub
        connections:
            pub_sub:
                host: 'noneRequired'
```

Usage
-----

You can directly use your queing system as before
