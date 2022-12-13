# Redocly API developer portal

## Prerequisites

* [node.js >= 12.22.6 and <= 16.x](https://nodejs.org/en/)
* [yarn](https://yarnpkg.com/en/)

{% swagger method="get" path="" baseUrl="https://example.com" summary="gives a list of users" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="query" name="limit" required="false" %}
Limit list of users, default 100, max 1000
{% endswagger-parameter %}

{% swagger-response status="200: OK" description="Success" %}
```javascript
{
    users: [
        {
            id: 1,
            name: "ds"
        },
        {
            id: 2,
            name: "as"
        }
    ]
}
```
{% endswagger-response %}

{% swagger-response status="500: Internal Server Error" description="Error" %}
```javascript
{
    // Response
}
```
{% endswagger-response %}
{% endswagger %}

## Install

```
yarn install
```

## Start development server

```
yarn start
```

Note: search isn't functional in the development environment.

## Troubleshooting

We heavily rely on caching for performance issues so if some changes are not reflected in the resulting portal try cleaning cache by running:

```
yarn clean
```

## Docs

Read the [online documentation](https://redoc.ly/docs/developer-portal/introduction/).

## Training program

The starter template contains training exercises which will teach you how to build a developer portal. After you start the development server, navigate to the app and follow the instructions to get started with your training.
