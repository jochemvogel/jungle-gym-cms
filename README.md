# JungleGym - CMS

CMS for the [JungleGym](https://github.com/iSirThijs/jungle-gym) application.

## :gear: Installation

### Developing

#### Install dependencies

```
yarn install
```

#### Run development server

```
yarn develop
```

### Environment Variables

Copy the `.env.example` and rename it to `.env`. Add your own database credentials

## :artist: Customise Admin

It's also possible to customise the layout of the CMS. For example things as colours, text and images. The Strapi admin panel is a React app that locates in the `node_modules/strapi-admin/admin/src` folder. You don't really need knowledge of React in order to edit the basic stuff.

If you want to edit a part, you need to copy the file (and the exact path) and put in the `admin/src` folder in the root of your project. The imported (npm) file will be overwritten. Be aware that you need to add **everything**, because the file will be overwritten. Don't just add some `background-color`, but copy the whole file and then update the `background-color`.

A quick way to copy a file is to use the command:

```
mkdir -p ./admin/src/containers/HomePage/ && cp ./node_modules/strapi-admin/admin/src/containers/HomePage/index.js ./admin/src/containers/HomePage/index.js
```

The text of the CMS is located in the `translations` folder. You can remove all the languages you don't use. For this project Dutch (`nl.json`) and English (`en.json`) will be used.

The Dutch translation is not that good, so you're free in changing that translation.

Read the whole documentation about editing in the [Strapi docs](https://strapi.io/documentation/developer-docs/latest/guides/custom-admin.html).

## Others

Add some documentation about the colors. Why the blue colors are green. This will be added later, but don't forget.
