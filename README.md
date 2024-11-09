<p align="center">
  <img width="auto" src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/master/img/header.svg?v=5" alt="Header">
</p>

<h3 align="center">

| [UpWork](https://www.upwork.com/freelancers/anthonybudd)  | [LinkedIn](https://www.linkedin.com/in/anthonybudd)  | [YouTube](https://www.youtube.com/@anthonycbudd) | [Instagram](https://www.instagram.com/anthonybudd.io) | [Calendly](https://calendly.com/anthonybudd/30min) |

</h3>

REST API & SaaS Specialist. Over 12 years of experience building web technology with PHP, TypeScript and JavaScript.

- ⭐️ My projects have generated over 1000 stars
- 🏢 Worked at Apple, RedHat and LegalZoom
- 🥇 UpWork Top Rated Developer
- ✅ Laravel Framework Contributor


<p align="center">
  <a href="https://www.youtube.com/watch?v=3rvBe_5Y78o">
  <img width="350" src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/master/img/6hr-startup-yt.png" alt="YouTube">
  </a>
</p>

<h6 align="center">

 [Coding a Live Start-up in 6hrs](https://youtu.be/3rvBe_5Y78o?si=b9UPv7suMAUyv5FP)  | [Frontend](https://github.com/anthonybudd/P.R.Box-UI)  | [Backend](https://github.com/anthonybudd/P.R.Box-API)

</h6>


# Work
<p align="center">
  <a href="https://www.upwork.com/freelancers/anthonybudd">
  <img width="auto" src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/master/img/banner.png?v=20-12-21" alt="HireMe">
  </a>
  </br>
  <!-- <a href="https://www.upwork.com/freelancers/anthonybudd">
  UpWork.com/freelancers/AnthonyBudd
  </a> -->
</p>

| <a href="https://www.upwork.com/services/product/development-it-on-prem-cryptocurrency-exchange-infrastructure-1729571406733246464"><img width="500" src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/master/img/product-infra.png?v=1"> I Can Build Your On-Prem Infrastructure.<br/>From $50,000</a> | <a href="https://www.upwork.com/services/product/development-it-bespoke-node-js-enterprise-grade-saas-mvp-1718712762925244416"><img width="500" src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/master/img/product-mvp.png?v=1"> I Can Build Your App in 28 days.<br/>From $15,000</a>|
| -- | -- |

<!-- <p align="center">
  <a href="https://www.upwork.com/freelancers/anthonybudd">
  UpWork.com/freelancers/AnthonyBudd
  </a>
</p> -->


# My Open-Source Projects

### [Express.ts API Template](https://github.com/anthonybudd/express-ts-api-template)

<a href="https://github.com/anthonybudd/express-ts-api-template"><img width="300" src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/master/img/express-ts-api-template.png"></a>

![Language](https://img.shields.io/badge/Language-Node.ts-success?style=flat)

Production-ready minimal REST API template using Express.js, Sequelize and MySQL.

- 👥 Users, Groups and Roles
- 🔐 Auth using JWT's with Passport.js
- 📄 MVC Code Generation
- 🌐 Production-ready [Kubernetes config files](https://github.com/anthonybudd/express-ts-api-template/blob/master/k8s/Deploy.md) and [OpenApiSpec.yml](https://github.com/anthonybudd/express-ts-api-template/blob/master/OpenApiSpec.yml)
- 🔌 Automated Client Library/SDK Generation with [openapi-generator-cli](https://github.com/OpenAPITools/openapi-generator-cli)
- 🥇 Real world tested, generated over $50M in revenue

| Method        | Route                                                    | Description                           | Payload                               | Response          | 
| ------------- | -------------------------------------------------------- | ------------------------------------- | ------------------------------------- | ----------------- |  
| `POST`        | `/api/v1/auth/login`                                     | Login                                 | `{email, password}`                     | `{accessToken}`     |  
| `POST`        | `/api/v1/auth/sign-up`                                   | Sign-up                               | `{email, password, firstName, tos}`     | `{accessToken}`     |  
| `GET`         | `/api/v1/user`                                           | Get the current user                  |                                         | `{User}`            |  
| `POST`        | `/api/v1/user`                                           | Update the current user               | `{firstName, lastName}`                 | `{User}`            |  
|               | [All Routes](https://github.com/anthonybudd/express-ts-api-template?tab=readme-ov-file#routes) |  |  |  |  


---

### [Vuetify 3 SaaS Template](https://github.com/anthonybudd/Vuetify3-SaaS-Template)

<a href="https://github.com/anthonybudd/Vuetify3-SaaS-Template">
  <img src="https://raw.githubusercontent.com/anthonybudd/Vuetify3-SaaS-Template/main/public/img/screenshots.png?v=1">
</a>

A minimal SaaS template built using Vuetify 3. Built to work out of the box with [AnthonyBudd/Express-TS-Api-Template](https://github.com/anthonybudd/express-ts-api-template) as the backend.

- 🔐 Login, Sign-up, ForgotPassword
- 📈 Dashboard
- 👥 Manage Account & Groups
- 💾 CRUD Model Example

```sh
git clone git@github.com:anthonybudd/Vuetify3-SaaS-Template.git
cd Vuetify3-SaaS-Template
cp .env.example .env
npm i
npm run dev
```

---

<a href="https://github.com/anthonybudd/s3-from-scratch">
  <img width="300" src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/master/img/s3.png">
</a>

### [An Attempt At Building Enterprise-grade S3 Infrastructure From Bare Metal](https://github.com/anthonybudd/s3-from-scratch)

Over the past few years I’ve been thinking about how I could build SaaS and deploy it on my own infrastructure without needing to use any cloud platforms like AWS or GCP. In this repo I document my progress on building a clone of AWS S3 that functions the same as S3 (automated bucket deployment, dynamically expanding volumes, security, etc) using an exclusively open-source technology stack.

---

<a href="https://github.com/anthonybudd/vipfs"><img width="300" src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/master/img/vipfs.png"></a>

### [VIPFS](https://github.com/anthonybudd/vipfs)
![Language](https://img.shields.io/badge/Language-Node.js-success?style=flat)
![Stars](https://img.shields.io/github/stars/anthonybudd/VIPFS?style=social)


VIPFS is a simple template project for creating permanent decentralised apps, blogs and websites that cannot be taken offline by anyone, including the government. VIPFS comes with useful templates and is pre-integrated with Bootstrap, FontAwesome and Video.js. Simply clone, compile and run  `npm run publish`  to deploy it on [IPFS](https://github.com/ipfs) and make your project permanently accesable to the world.

- [YouTube Tutorial](https://www.youtube.com/watch?v=Fq7h-cSN9i8)
- Featured on [MadeWithVueJS.com](https://madewithvuejs.com/vipfs)
- Featured on [BestOfVue.com](https://bestofvue.com/repo/Ideea-inc-vipfs)

---

<a href="https://github.com/anthonybudd/Open-Source-Crypto-ATM"><img width="300" src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/master/img/osca.jpg"></a>


### [OSCA. Open-Source Crypto ATM](https://github.com/anthonybudd/Open-Source-Crypto-ATM)
![Stars](https://img.shields.io/github/stars/anthonybudd/Open-Source-Crypto-ATM?style=social)


A crypto-currency ATM that someone with minimal electro-mechanical skill can build at home with parts from Amazon and hardware from Lowes. The user inserts cash and the machine returns a cold wallet loaded with the desired amount of crypto-currency. OSCA does not require you to disclose any personal information to use this ATM.

---

<p>
  <a href="https://github.com/anthonybudd/larachan"><img width="300" src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/master/img/larachan.png"></a>
</p>

### [LaraChan](https://github.com/anthonybudd/larachan)
![Language](https://img.shields.io/badge/Language-PHP-success?style=flat) ![Stars](https://img.shields.io/github/stars/anthonybudd/larachan?style=social)


LaraChan is a simple 4chan-style imageboard built on Laravel 8. The project can be installed in 5 easy commands and is designed to be deployed on a Raspberry Pi. Many useful Artisan commands are provided so you can administrate your imageboard using the CLI.

- 🧅 **Tor**  - DarkWeb ready. Built-in Tor proxy.
- 🤖 **CAPTCHA**  - Self-hosted captchas.
- 🚫 **No .JS**  - No front-end Java-Script.

&nbsp;&nbsp;&nbsp;&nbsp;

--- 

<a href="https://github.com/anthonybudd/camera-spike"><img src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/main/img/camera-spike.png?v=1"></a>


### [Camera Spike](https://github.com/anthonybudd/Camera-Spike)
![Language](https://img.shields.io/badge/Language-Node.js-success?style=flat)
![Stars](https://img.shields.io/github/stars/anthonybudd/Camera-Spike?style=social)


Camera Spike is a basic self-hosted security camera project for the Raspberry Pi. A web UI is provided using Tor, this allows you to remotely monitor the feed without needing to register the device with a 3rd-party or without disclosing your IP address or the IP address of the Camera Spike. CLI tools are provided so you can easily create a custom onion v3 address.

&nbsp;&nbsp;&nbsp;&nbsp;

---

<a href="https://github.com/anthonybudd/s4"><img width="300" src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/master/img/s4.png"></a>


### [S4](https://github.com/anthonybudd/s4)
![Stars](https://img.shields.io/github/stars/anthonybudd/s4?style=social)


S4 is 100% compatible AWS S3 storage, accessed through Tor and distributed using IPFS. Tor acts as a DNS and [IPFS](https://github.com/ipfs/ipfs) acts as a CDN and will make your data permanently accessible and is almost impossible to take offline. A [sidecar docker container](https://github.com/anthonybudd/s4-client) is provided to seamlessly proxy requests from your existing S3 code over Tor to S4. Basically it's self-hosted S3 that also makes the data accessible on IPFS.


- [YouTube Tutorial](https://youtu.be/RMNjpAmCvcQ)
- [Talking about S4 on the IPFS weekly meet-up](https://www.youtube.com/watch?v=8F62oXVrYJU)

---

<a href="https://github.com/anthonybudd/nginx-tor-proxy"><img height="75" src="https://github.com/anthonybudd/nginx-tor-proxy/raw/master/docs/img/header.png"></a>

### [NGINX TOR Proxy](https://github.com/anthonybudd/nginx-tor-proxy)


NGINX Tor Proxy is a simple container that exposes your containers with a custom Tor v3 Onion address.

Tor vanity URLs generated using [cathugger/mkp224o](https://github.com/cathugger/mkp224o)

<!-- ---

### [CLI Password Manager](https://github.com/anthonybudd/CLI-Password-Manager)

CLI Password Manager gives you 4 simple commands for easily encrypting and decrypting a local password vault using OpenSSL.

```js
clipm-dec
clipm-nano
clipm-enc
``` -->

---

<!-- ### [If](https://github.com/anthonybudd/If)

A chainabale if library for JavaScript.

This is totally pointless, I just wanted to see if I could build this because I think this kind of chainable syntax looks better over control-structure syntax in the `.then()` method of a promise.

```js
const myArr = ['a', 'b', 'c'];
const result = new If(myArr.length < 2)
    .then(() => ('Array less than 2'))
    .elseif((myArr.length > 3), () => ('Array greater than 3'))
    .else(() => ('Array has length 3'))
    .fi();

console.log(result); // 'Array has length 3'
```



--- -->


### Archived Projects

#### [WP_Model](https://github.com/anthonybudd/wp_model)
![Language](https://img.shields.io/badge/Language-PHP-success?style=flat) ![Stars](https://img.shields.io/github/stars/anthonybudd/wp_model?style=social)


WP_Model is an advanced pseudo ORM for WordPress, it provides active-record models of WordPress posts in the style of Laravel's ORM eloquent.

```PHP
Class Product extends WP_Model
{
    public $postType = 'product';
    public $attributes = [
        'color',
        'price'
    ];
}

Product::register();

$book = new Product;
$book->title = 'WordPress for dummies';
$book->color = 'Yellow';
$book->price = 20;
$book->save();
```


#### [WP_Route](https://github.com/anthonybudd/wp_route)
![Language](https://img.shields.io/badge/Language-PHP-success?style=flat) ![Stars](https://img.shields.io/github/stars/anthonybudd/wp_route?style=social)


WP_Route is a simple way to create custom routes in WordPress for listening for webhooks, oAuth callbacks and basic routing. WP_Route is a single class solution that supports route parameters and redirects and does not require any set-up.
```PHP
WP_Route::get('flights',                        'listFlights');
WP_Route::post('flights/{flight}',              'singleFlight');
WP_Route::put('flights/{flight}/book/{date}',   'bookFlight');
WP_Route::delete('flights/{flight}/delete',     'deleteFlight');

WP_Route::any('flights/{flight}',               array('Class', 'staticMethod'));
WP_Route::patch('flights/{flight}',             array($object, 'method'));
WP_Route::match(['get', 'post'],                'flights/{flight}/confirm', 'confirmFlight');
WP_Route::redirect('/from/here',                '/to/here', 301);
```



#### [WP_Mail](https://github.com/anthonybudd/wp_mail)
![Language](https://img.shields.io/badge/Language-PHP-success?style=flat) ![Stars](https://img.shields.io/github/stars/anthonybudd/wp_mail?style=social)


WP_Mail is the simplest and most powerful dynamic email class available for WordPress. The class provides simple methods for attaching files, custom headers and lots of helper functions. The class only sends emails using the WordPress function wp_mail(), this means that all of your existing SMTP settings will continue to work with no additional config or set-up required.
```PHP
$email = WP_Mail::init()
    ->to('john.doe@gmail.com')
    ->subject('WP_Mail is great!')
    ->template(get_template_directory() .'/emails/example.php', [
        'name'     => 'Anthony Budd',
        'location' => 'London',
        'skills'   => [
           'PHP',
           'AWS',
        ] 
    ])
    ->send();
```



🟨⬛️🐍
