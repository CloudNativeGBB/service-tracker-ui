# ![alt text](https://github.com/CloudNativeGBB/arcdemo-service-tracker-ui/blob/master/src/assets/img/msft_logo_24.png "Microsoft Intelligent Cloud Global Blackbelt") &nbsp;service-tracker-ui <sup style='font-size:12px'>&nbsp;&nbsp;cloudnativegbb/service-tracker-ui</sup>

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

Service setup <sup style='font-size:11px'>or adding services</sup>
----------

[Webpack Proxy Config](./vue.config.js)

This lists the proxy location for services

> e.g., &nbsp;&nbsp; ***/api/flights/inair*** 
```javascript
    '/api/flights/inair':{
        target: 'http://localhost:8004',
        changeOrigin: true,
        pathRewrite: {
          '^/api/flights/inair': '/api/stats/flights/inair'
        }
    }
```

Built with
------

[Vue Paper Dashboard](https://cristijora.github.io/vue-paper-dashboard/)
