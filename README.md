Yii2.x extension of UnSlider 
=============================
a wrapper of UnSlider for Yii2.x Framework

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist rogeecn/yii2-unslider "~1.0.1"
```

or add

```
"rogeecn/yii2-unslider": "*"
```

to the require section of your `composer.json` file.


Usage
-----

Once the extension is installed, simply use it in your code by  :

```php
<?= \rogeecn\UnSlider\Slider::widget([
    'slides' => [
        [
            'body' => 'Unslider widget for Yii2', // body will work when image field is not exist
            'url'  => "#",
        ],
        [
            'body' => $this->render("_body_view"), // you can render html instead
        ],
        [
            'image'   => '/images/cat2.jpg',
            'body'  => 'description',
        ],
    ],

]); ?>
```