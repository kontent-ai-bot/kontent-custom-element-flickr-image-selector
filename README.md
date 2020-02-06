# Flickr Image Selector Custom Element for Kentico Kontent

This is a [custom element](https://docs.kontent.ai/tutorials/develop-apps/integrate/integrating-your-own-content-editing-features) for [Kentico Kontent](https://kontent.ai) that allows users search images on Flickr and select one. **NOTE: Selected image may be subject to copyright and/or usage restrictions.**

![Screenshot of custom element](FlickrImageSelector.gif)

## Setup

1. Get an [API key for Flickr](https://www.flickr.com/services/developer/api/)
1. Deploy the code to a secure public host
    * See [deploying section](#Deploying) for a really quick option
1. Follow the instructions in the [Kentico Kontent documentation](https://docs.kontent.ai/tutorials/develop-apps/integrate/integrating-your-own-content-editing-features#a-3--displaying-a-custom-element-in-kentico-kontent) to add the element to a content model.
    * The `Hosted code URL` is where you deployed to in step 1
    * Pass the necessary parameters as directing in the [JSON Parameters configuration](#json-parameters) section of this readme.

## Deploying

Netlify has made this easy. If you click the deploy button below, it will guide you through the process of deploying it to Netlify and leave you with a copy of the repository in your GitHub account as well.

***UPDATE THE REPOSITORY URL BELOW***

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/ChristopherJennings/kontent-custom-element-sample-template)

## JSON Parameters

the `apiKey` property is required. This is your [Flickr API key](https://www.flickr.com/services/developer/api/).

```Json
{
  "apiKey": "[YOUR KEY]"
}
```

## Saved Value

The value is saved as a string representing the URL of the selected image.

## Contributors

Originally contributed by [@maartenvdh](https://github.com/maartenvdh/)
