# Пример json-разметки BreadcrumbList в JSON-LD
```js
<script type="application/ld+json">
    {
        "@context": "http://schema.org",
        "@type": "BreadcrumbList",
        "itemListElement":
        [
            {"@type": "ListItem",
            "position": 1,
            "item":
                {"@id": "https://artzolin.ru/",
                "name": "Zolin Digital"}
            },
            {"@type": "ListItem",
            "position": 2,
            "item":
                {"@id": "https://artzolin.ru/category/articles/",
                "name": "Статьи"}
            },
            {"@type": "ListItem",
            "position": 3,
            "item":
                {"@id": "https://artzolin.ru/articles/schema-snippets/",
                "name": "Schema Snippets"}
            }
        ]
    }
</script>
```

# Пример json-разметки Organization в JSON-LD
```js
<script type="application/ld+json">
    {
        "@context": "http://schema.org",
        "@type": "Organization",
        "address": {
            "@type": "PostalAddress",
            "addressLocality": "Москва, Россия",
            "postalCode": "105264",
            "streetAddress": "5-ая Парковая, 52"
        },
        "email": "pochta@medvedica.org",
        "name": "Медведица",
        "telephone": "+7 (495) 223 45 45"
    }
</script>
```

# Пример json-разметки LocalBusiness в JSON-LD
```js
<script type="application/ld+json">
    {
        "@context": "http://schema.org",
        "@type": "LocalBusiness",
        "additionalType": "AutoRental",
        "address": {
            "@type": "PostalAddress",
            "addressLocality": "Москва",
            "streetAddress": "ул. Илимская, дом 1 Б"
        },
        "name": "Абсолют Корона",
        "email": "mail@absolutecrown.ru",
        "openingHours": [
            "Mo-Fr 10:00-21:00",
            "Sa-Su 10:00-18:00"
        ],
        "priceRange": "1100-4700RUB",
        "telephone": [
            "8 (495) 783-70-83",
            "8 (916) 783-03-03"
        ],
        "image": "/images/logo-square.png",
        "url": "https://www.absolutecrown.ru",
        "geo": {
            "@type": "GeoCoordinates",
            "latitude": "55.88923006884247",
            "longitude": "37.57312349999997"
        }
    }
</script>
```

# Пример json-разметки QApage в JSON-LD
```js
<script type="application/ld+json">
    {
        "@context": "https://schema.org/",
        "@type": "Product",
        "name": "Dorothy Perkins Свитер",
        "image": [
            "https://shop.com/photos/1x1/photo.jpg",
            "https://shop.com/photos/4x3/photo.jpg"
        ],
        "description": "Теплый свитер синего цвета из 100% мериносовой шерсти.",
        "sku": "0446310786",
        "brand": {
            "@type": "Thing",
            "name": "Dorothy Perkins"
        },
        "aggregateRating": {
            "@type": "AggregateRating",
            "ratingValue": "4.4",
            "reviewCount": "89"
        },
        "offers": {
            "@type": "Offer",
            "url": "https://shop.com/dp-sviter",
            "priceCurrency": "RUB",
            "price": "2500",
            "priceValidUntil": "2020-11-05",
            "itemCondition": "https://schema.org/NewCondition",
            "availability": "https://schema.org/InStock",
            "seller": {
                "@type": "Organization",
                "name": "Интернет-магазин Shop.co"
            }
        }
    }
</script>
```

# Пример json-разметки Article в JSON-LD
```js
<script type="application/ld+json">
    {
        "@context": "http://schema.org/",
        "@type": "Article",
        "headline": "Аквариумные рыбы лисицы",
        "image": "https://www.aqua-shop.ru/images/news/Siganus_vulpinus-Lo.jpg",
        "description": "Лисицы — весьма распространенные рыбы в морской аквариумистике. Принадлежат к одноимённому семейству Рыбы-лисицы. Встречаются в водах Индо-Пацифики и Средиземноморья.",
        "author": "Аква Шоп",
        "publisher": {
            "@type": "Organization",
            "name": "aqua-shop.ru",
            "url": "https://www.aqua-shop.ru",
            "logo": {
                "@type": "ImageObject",
                "url": "https://www.aqua-shop.ru/images/news/logo_Aqua-shop.jpg"
            }
        },
        "datepublished": "2016-03-21",
        "datemodified": "2018-05-22",
        "mainEntityOfPage": {
            "@type": "WebPage",
            "@id": "https://www.aqua-shop.ru/articles/rybki_lisicy"
        }
    }
</script>
```

# Пример json-разметки поисковой строки в JSON-LD
```js
<script type="application/ld+json">
    {
        "@context": "http://schema.org",
        "@type": "WebSite",
        "url": "https://rider-skill.ru/",
        "potentialAction": {
            "@type": "SearchAction",
            "target": "https://rider-skill.ru/?s={query}",
            "query-input": "required name=query"
        }
    }
</script>
```

# Пример json-разметки FAQpage в JSON-LD
```js
<script type="application/ld+json">
    {
        "@context": "https://schema.org",
        "@type": "FAQPage",
        "mainEntity": [{
            "@type": "Question",
            "name": "✅ Когда можно обратиться в офис?",
            "acceptedAnswer": {
                "@type": "Answer",
                "@id":"a1",
                "text": "Мы работаем без выходных и перерывов на обед. Время работы нашего офиса: пн, вт, ср, чт, пт – 10:00-20:00, сб, вс – 10:00-17:00."
            }
        }, {
            "@type": "Question",
            "name": "✅ Можно ли осмотреть Ваши автомашины и как это сделать?",
            "acceptedAnswer": {
                "@type": "Answer",
                "@id":"a2",
                "text": "Осмотр автомобилей производится в нашем автопарке до заключения договора и оплаты. Типовой договор Вы можете найти <a href=\"/link\">по ссылке</a>."
            }
        }]
    }
</script>
```

# Пример json-разметки QApage в JSON-LD
```js
<script type="application/ld+json">
    {
        "@context": "https://schema.org",
        "@type": "QAPage",
        "mainEntity": {
            "@type": "Question",
            "name": "Как много пальцев у кошки?",
            "text": "Интересно, как много пальцев у кошек на лапках?",
            "answerCount": 3,
            "upvoteCount": 26,
            "dateCreated": "2019-07-23",
            "author": {
                "@type": "Person",
                "name": "Ваня Иванов"
            },
            "acceptedAnswer": {
                "@type": "Answer",
                "text": "В норме у кошачьих 18 пальцев: по 5 на передних лапках и по 4 на задних. Но у кошек широко распространена полидактилия. У знаменитых кошек Хэмингуэя, живущих в его доме на Кубе, на передних лапах по 6 пальцев и больше.",
                "dateCreated": "2019-11-02",
                "upvoteCount": 1337,
                "url": "https://voprosy.com/question1#acceptedAnswer",
                "author": {
                    "@type": "Person",
                    "name": "Алексей Котиков"
                }
            },
            "suggestedAnswer": [
                {
                    "@type": "Answer",
                    "text": "Столько же, сколько у собак.",
                    "dateCreated": "2019-11-04",
                    "upvoteCount": 42,
                    "url": "https://voprosy.com/question1#suggestedAnswer1",
                    "author": {
                        "@type": "Person",
                        "name": "Михаил Собачкин"
                    }
                }
            ]
        }
    }
</script>
```