# ![alt text](https://github.com/CloudNativeGBB/arcdemo-service-tracker-ui/blob/master/src/assets/img/msft_logo_24.png "Microsoft Intelligent Cloud Global Blackbelt") &nbsp;service-tracker-ui 

Requirements
----------
> service-tracker-ui uses the following 
* [Nodejs](https://nodejs.org)
* [Vue CLI](https://vuejs.org)

Run it locally
---------- 

> Install Dependencies

```bash
npm install
```

> Run with npm (this serves with the vue-cli and webpack)

```bash
npm run dev
```

Service setup 
----------

[Webpack Proxy Config](./vue.config.js)


> e.g., &nbsp;&nbsp; ***/api/flights/inair*** 
```javascript
    '/api/flights/santa-claus':{
        target: 'http://localhost:8004',
        changeOrigin: true,
        pathRewrite: {
          '^/api/flights/santa-claus': '/api/stats/flights/santa-claus'
        }
    }
```

Built with
------

[Vue Paper Dashboard](https://cristijora.github.io/vue-paper-dashboard/)
