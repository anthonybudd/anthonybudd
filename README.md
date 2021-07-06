<p align="center">
  <img width="auto" src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/master/img/header.svg" alt="Header">
</p>

I am an expert Node.js and PHP developer with over 10 years of commercial experience building, deploying and maintaing REST APIs.

- ⭐️ My projects have generated over 650 stars
- 🤓 Worked at Apple, RedHat and LegalZoom
- ✅ Laravel Framework Contributor [PR:28849](https://github.com/laravel/framework/pull/28849) merged by [Taylor Otwell](https://github.com/taylorotwell)


#### Hire Me
I am currently available for hire at a rate of $90 USD/hr. Please send a project brief to [anthonybudd94@gmail.com](mailto:anthonybudd94@gmail.com?subject=We%20would%20like%20to%20hire%20you.) for a quote.


---

<p>
  <a href="https://github.com/anthonybudd/vipfs"><img width="300" align='right' src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/master/img/vipfs.png"></a>
</p>

### [VIPFS](https://github.com/anthonybudd/vipfs)
![Language](https://img.shields.io/badge/Language-Node.js-success?style=flat)
![Stars](https://img.shields.io/github/stars/anthonybudd/VIPFS?style=social)


VIPFS is a simple boilerplate project for creating permanent decentralised apps, blogs and websites that cannot be taken offline by anyone, including the government. VIPFS comes with useful templates and is pre-integrated with Bootstrap, FontAwesome and Video.js. Simply clone, compile and run  `npm run publish`  to deploy it on [IPFS](https://github.com/ipfs) and make your project permanently accesable to the world.

- [YouTube Tutorial](https://www.youtube.com/watch?v=Fq7h-cSN9i8)
- Featured on [MadeWithVueJS.com](https://madewithvuejs.com/vipfs)

---
<p>
  <a href="https://github.com/anthonybudd/larachan"><img width="300" align='right' src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/master/img/larachan.png"></a>
</p>

### [LaraChan](https://github.com/anthonybudd/larachan)
![Language](https://img.shields.io/badge/Language-PHP-success?style=flat) ![Stars](https://img.shields.io/github/stars/anthonybudd/larachan?style=social)


LaraChan is a simple 4chan-style imageboard built on Laravel 8. The project can be installed in 5 easy commands and is designed to be deployed on a Raspberry Pi. Many of useful Artisan commands are provided so you can administrate your imageboard using the CLI.

- 🧅  **Tor**  - Built in Tor proxy
- 🤖  **CAPTCHA**  - Self-hosted captchas.
- 🚫  **No .JS**  - No front-end JavaScript.

---
<p>
  <a href="https://github.com/anthonybudd/s4"><img width="300" align='right' src="https://raw.githubusercontent.com/anthonybudd/anthonybudd/master/img/s4.png"></a>
</p>

### [S4](https://github.com/anthonybudd/s4)


![Stars](https://img.shields.io/github/stars/anthonybudd/s4?style=social)
S4 is 100% compatible AWS S3 storage, accessed through Tor and distributed using IPFS. Tor acts as a DNS and [IPFS](https://github.com/ipfs/ipfs) acts as a CDN and will make your data permanently accessible and is almost impossible to take offline once it has been published. A [sidecar docker container](https://github.com/anthonybudd/s4-client)  is provided to seamlessly proxy requests from your existing S3 code over Tor to S4.


- [YouTube Tutorial](https://youtu.be/RMNjpAmCvcQ)
- [Talking about S4 on the IPFS weekly meet-up](https://www.youtube.com/watch?v=8F62oXVrYJU)


---
### Archived Projects

#### [WP_Model](https://github.com/anthonybudd/wp_model)
![Language](https://img.shields.io/badge/Language-PHP-success?style=flat) ![Stars](https://img.shields.io/github/stars/anthonybudd/wp_model?style=social)


WP_Model is a pseudo ORM for WordPress, it provides an eloquent-esque active record style models of WordPress posts. 

```PHP
Class Product extends WP_Model
{
    public $postType = 'product';
    public $attributes = [
        'color',
        'weight'
    ];
}

Product::register();

$book = new Product;
$book->title = 'WordPress for dummies';
$book->color = 'Yellow';
$book->weight = 100;
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
WP_Route::redirect('/from/here',                 '/to/here', 301);
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
