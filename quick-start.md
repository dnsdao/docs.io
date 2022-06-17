# Quick Start



{% hint style="info" %}
**Good to know:** A quick start guide can be good to help folks get up and running with your API in a few steps. Some people prefer diving in with the basics rather than meticulously reading every page of documentation!
{% endhint %}

## Get your API keys

Your API requests are authenticated using API keys. Any request that doesn't include an API key will return an error.

You can generate an API key from your Dashboard at any time.

The best way to interact with our API is to use one of our official libraries:

{% hint style="info" %}
**Good to know:** Using tabs to separate out different languages is a great way to present technical examples or code documentation without cramming your docs with extra sections or pages per language.
{% endhint %}

## Make your first request

To make your first request, send an authenticated request to the pets endpoint. This will create a `pet`, which is nice.

{% swagger baseUrl="/dns/name" method="get" path="" summary="Reverse DNS" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="body" name="name" required="true" type="string" %}
The  domain name
{% endswagger-parameter %}

{% swagger-response status="200" description="Pet successfully created" %}
{ "name": "asimov.com", "nameHash": "d339810ebe769de83bcc884b2d07c32e90432c2fd9049bbb692cb6f8ab140f9c", "rootHash": "b5fcf7e95d62d6d62a9de5c98619595652bd6d90a3ef4a4b23bde43cb10e3035", "owner": "d07bdb622a7e9d519a17c4c097bc479012761880", "expireTime": 1684488247, "conf": { "A": "", "AAAA": "", "BlockChain": "", "CName": "", "IOTA": "", "MX": "", "MXBCA": "", "Optional": "" }, "root": { "name": "com", "hash": "b5fcf7e95d62d6d62a9de5c98619595652bd6d90a3ef4a4b23bde43cb10e3035", "isCustom": false, "customPrice": 4000000000000000000, "isOpen": true, "owner": "6181c756e51ff37869b8b7678c4c956a1a2f5073", "expireTime": 1683595911, "conf": { "A": "", "AAAA": "", "BlockChain": "", "CName": "", "IOTA": "", "MX": "", "MXBCA": "", "Optional": "" } } }
{% endswagger-response %}

{% swagger-response status="401" description="Permission denied" %}

{% endswagger-response %}
{% endswagger %}

{% hint style="info" %}
**Good to know:** You can use the API Method block to fully document an API method. You can also sync your API blocks with an OpenAPI file or URL to auto-populate them.
{% endhint %}

Take a look at how you might call this method using our official libraries, or via `curl`:
