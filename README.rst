Amazon Scraper Python
========================

Python SDK that allows scraping Amazon products data and Amazon products
reviews

`API Docs <https://app.outscraper.com/api-docs#tag/Amazon>`__

`Generate API Token <https://app.outscraper.com/profile>`__

Installation
------------

Python 3+

.. code:: bash

   pip install amazon-scraper

`Link to the python package
page <https://pypi.org/project/google-maps-reviews/>`__

Initialization
--------------

.. code:: python

   from amazon_scraper_by_outscraper import AmazonClient

   client = AmazonClient(api_key='SECRET_API_KEY')

Scrape Amazon Products
----------------------

.. code:: python

   # Get data by prodcut URL
   results = client.get_prodcuts('https://www.amazon.com/dp/1612680194')

   # Get data from summary page
   results = client.get_prodcuts('https://www.amazon.com/s?k=iphone', limit=24)

Scrape Amazon Reviews
---------------------

.. code:: python

   # Get reviews from Amazon product by URL
   results = client.get_reviews('https://www.amazon.com/dp/1612680194', limit=3)

   # Get reviews from Amazon product by ASIN
   results = client.get_reviews('1612680194', limit=3)

Amazon Products Results Demo
----------------------------

.. code:: json

   {
     "id": "your-request-id",
     "status": "Success",
     "data": [
       [
         {
           "short_url": "https://www.amazon.com/Lacoste-Womens-Stainless-Leather-Calfskin/dp/B00G3XWLR8",
           "asin": "B00G3XWLR8",
           "name": "Lacoste Women's 12.12 Stainless Steel Quartz Watch with Leather Calfskin Strap, Taupe, 16 (Model: 2001150)",
           "rating": null,
           "reviews": null,
           "answered_questions": null,
           "fast_track_message": null,
           "about": "ON TIME, IN STYLE: Once upon a time there was a polo shirt that made history now it has inspired a ladies timepiece to follow in its footsteps. The Lacoste.12.12 Lady is the epitome of sporty chic and comfort, with thoughtful dashes of detail. Game, set and match for style., QUALITY MATERIALS: Women's 36 mm pale rose gold ion-plated stainless steel case with a taupe leather strap featuring a carnation gold dial., QUARTZ MULTIFUNCTION: It’s a battery-powered watch that sends energy through a quartz crystal. Is typically built into three separate dials for the day of the week, date of the month and 24-hour time., DURABLE MINERAL CRYSTAL: Made from glass and protects watch from scratches., 2 YEAR WARRANTY: Lacoste offers a 2-year limited warranty against defects in materials and workmanship that prevent the watch from functioning properly under normal use. Only purchases from an authorized retailer are covered by the manufacturer’s warranty.",
           "description": "The Lacoste legend was born in 1933, when Rene Lacoste revolutionized men's fashion replacing the classical woven fabric, long-sleeved and starched shirts on the courts, by what has now become the classic LACOSTE polo shirt. More than 75 years after its creation, LACOSTE has become a lifestyle brand which allies elegance and comfort. The LACOSTE art of living expresses itself today through a large collection of apparel for women, men and children, footwear, fragrances, leather goods, eyewear, watches, belts, home textiles, and fashion jewelry. LACOSTE founds its success on the essential values of authenticity, performance, and elegance. The crocodile incarnates today the elegance of the champion, Rene Lacoste, as well as of his wife Simone Lacoste and their daughter Catherine Lacoste, both also champions, in everyday life as on the tennis courts and golf courses. The Crocodile's origins The true story of the \"Crocodile\" begins in 1923 after a bet that Rene Lacoste had with the Captain of the French Davis Cup Team, Allan H. Muhr, who promised him an alligator suitcase if he won an important game for the team. This episode was reported in an article in the Boston Evening Transcript, where his nickname of the Crocodile came to life for the first time. The American public grew fond of this nickname which highlighted the tenacity he displayed on the tennis courts, never giving up his prey. His friend Robert George drew him a crocodile which was embroidered on the blazer he wore on the courts. The Legend was born.",
           "categories": [
             "Clothing, Shoes & Jewelry",
             "Women",
             "Watches",
             "Wrist Watches"
           ],
           "store_title": "Lacoste Store",
           "store_url": "https://www.amazon.com/stores/Lacoste/page/C85490CB-0E64-4F8B-89A8-217111AFF6FE?ref_=ast_bln",
           "price": "$175.00",
           "availability": "In stock soon. Order it now.",
           "strike_price": null,
           "price_saving": null,
           "shipping": "",
           "merchant_info": "",
           "bage": "",
           "currency": null,
           "image_1": "https://m.media-amazon.com/images/I/314jzz9RfsL.jpg",
           "image_2": "https://m.media-amazon.com/images/I/31he4kecs0L.jpg",
           "image_3": "https://m.media-amazon.com/images/I/31FgebhbXEL.jpg",
           "image_4": "https://m.media-amazon.com/images/I/41IYiTJyLIL.jpg",
           "image_5": "https://m.media-amazon.com/images/I/41gZMv+FwoL.jpg",
           "overview": null,
           "details": {
             "details.brand_seller_or_collection_name": "Lacoste",
             "details.model_number": "2001150",
             "details.part_number": "2001150",
             "details.item_shape": "Round",
             "details.dial_window_material_type": "Mineral",
             "details.display_type": "Analog",
             "details.clasp": "Tang Buckle",
             "details.case_material": "Stainless Steel",
             "details.case_diameter": "36 millimeters",
             "details.case_thickness": "9.75 millimeters",
             "details.band_material": "Leather",
             "details.band_size": "Womens Standard",
             "details.band_width": "16 millimeters",
             "details.band_color": "Brown",
             "details.dial_color": "Carnation Gold",
             "details.bezel_material": "Stainless Steel",
             "details.bezel_function": "Stationary",
             "details.calendar": "Day-Date",
             "details.movement": "Quartz",
             "details.water_resistant_depth": "50 Meters",
             "details.warranty": "Manufacturer’s warranty can be requested from customer service. to make a request to customer service.",
             "details.package_dimensions\n‏\n\n‎": "3.58 x 3.46 x 3.23 inches; 3.84 Ounces",
             "details.item_model_number\n‏\n\n‎": "2001150",
             "details.department\n‏\n\n‎": "Womens",
             "details.date_first_available\n‏\n\n‎": "January 13, 2021",
             "details.manufacturer\n‏\n\n‎": "Lacoste",
             "details.asin\n‏\n\n‎": "B00G3XWLR8",
             "details.country_of_origin\n‏\n\n‎": "China"
           }
         }
       ]
     ]
   }

.. _amazon-products-results-demo-1:

Amazon Products Results Demo
----------------------------

.. code:: json

   {
     "id": "your-request-id",
     "status": "Success",
     "data": [
       [
         {
           "query": "https://www.amazon.com/dp/1612680194",
           "id": "R2VYT9ETWPTAWU",
           "product_asin": "1612680194",
           "title": "Everything",
           "body": "I read this book about 11 years ago at 27 years old , had no money, I followed the advice in this book and now have 15 rental properties paid off free and clear, my assets more than cover all my expenses. I just bought this book again, I'm in the middle of reading it again now 11 years later and can't put it down.  I hate reading btw.  I plan on reading this book at least three more times over the next 20 years so I can keep all info fresh in my mind. People always ask me about success. I tell them to read this book...whats crazy is that they don't read it. You can lead a horse to water but can't make it drink. The book changed my life and it will change yours. Do you want change or do you just want to talk and think about change? There is a big difference , do it.",
           "rating": 5,
           "rating_text": "5.0 out of 5 stars",
           "helpful": "1,331 people found this helpful",
           "comments": null,
           "date": "Reviewed in the United States on March 17, 2018",
           "bage": "Verified Purchase",
           "official_comment_banner": "",
           "url": "https://www.amazon.com/gp/customer-reviews/R2VYT9ETWPTAWU/ref=cm_cr_arp_d_rvw_ttl?ie=UTF8&ASIN=1612680194",
           "img_url": null,
           "variation": "",
           "total_reviews": 65459,
           "overall_rating": 4.7,
           "author_title": "Ilive4him24",
           "author_descriptor": "",
           "author_url": "https://www.amazon.com/gp/profile/amzn1.account.AGQCR5JZP3V6Y743KX3UYJBRRVOA/ref=cm_cr_arp_d_gw_btm?ie=UTF8",
           "author_profile_img": "https://images-na.ssl-images-amazon.com/images/S/amazon-avatars/default._CR0,0,1024,1024_SX48_.png",
           "product_name": "Rich Dad Poor Dad: What the Rich Teach Their Kids About Money That the Poor and Middle Class Do Not!",
           "product_url": "https://www.amazon.com/dp/1612680194"
         },
         {
           "query": "https://www.amazon.com/dp/1612680194",
           "id": "R1T9953QMMGUEX",
           "product_asin": "1612680194",
           "title": "Make sure you Select the Book Size",
           "body": "I owned this book in the past and wanted to reorder it to read it again.  Instead of getting the book I expected, I received a tiny, hand sized book, with print that is too small and that is, frankly, hard to open all the way in order to read the words near the binder.  So the book is utterly useless. With all the complaints about this tiny book, I'm not sure why that is the book that automatically comes up when you search for the book.  Instead, the normal sized book should be the default, and then people can select the pocket sized book if they want. So I would say that the content of the book is excellent. DO purchase the book; however, BE SURE TO SELECT THE LARGER, PAPERBACK VERSION if that's what you want (sorry for the all caps, just want to make sure people see that part).",
           "rating": 1,
           "rating_text": "1.0 out of 5 stars",
           "helpful": "851 people found this helpful",
           "comments": null,
           "date": "Reviewed in the United States on January 23, 2018",
           "bage": "Verified Purchase",
           "official_comment_banner": "",
           "url": "https://www.amazon.com/gp/customer-reviews/R1T9953QMMGUEX/ref=cm_cr_arp_d_rvw_ttl?ie=UTF8&ASIN=1612680194",
           "img_url": null,
           "variation": "",
           "total_reviews": 65459,
           "overall_rating": 4.7,
           "author_title": "judysardenspeaker",
           "author_descriptor": "",
           "author_url": "https://www.amazon.com/gp/profile/amzn1.account.AHBNQFY6SXYTRVWW7RUKDYY4RBBA/ref=cm_cr_arp_d_gw_btm?ie=UTF8",
           "author_profile_img": "https://images-na.ssl-images-amazon.com/images/S/amazon-avatars-global/default._CR0,0,1024,1024_SX48_.png",
           "product_name": "Rich Dad Poor Dad: What the Rich Teach Their Kids About Money That the Poor and Middle Class Do Not!",
           "product_url": "https://www.amazon.com/dp/1612680194"
         },
         {
           "query": "https://www.amazon.com/dp/1612680194",
           "id": "RIGBUZ8E2S6UT",
           "product_asin": "1612680194",
           "title": "A great foundation book for beginning to improve your financial intelligence",
           "body": "This is an enhanced reprint of the original, with additional study questions/ discussion and review added at the end of every chapter. I bought the original about 18 years ago and it changed my families destiny for the better. I am glad the reprint came out as it prompted me to reread it and deepen my understanding. Some people complain that this book does not give a step by step process for change. I would counter that one size shoe does not fit all feet. There are many individual paths to wealth, and Kiyosaki sets the guiding stars to navigate by, but you have to walk your own individual road. Some key concepts of this book are: 1) Assets put money in your pocket even when you are on vacation. Liabilities take money out of your pocket, therefore your house is a liability [unless you rent out rooms and the garage as one person I know did while rebuilding his asset base]. 2) Wealthy people buy assets first, and then let their assets buy their luxuries from the surplus cash flow. 3) Wealthy people continuously increase their assets by reinvesting their surplus cash flow in more assets. 4) There are 3 primary asset classes: Real Estate, Businesses, and Paper assets (stocks bonds notes, etc) 5) Cash Flow is more important than Net Worth. Net Worth is similar to potential energy, to use it you have to spend it, then it is gone. Cash Flow is like power from a hydroelectric dam, constantly replenished. The rich don't work for money, they work for assets. The tax laws are fair from the standpoint that the laws that the rich spent billions of dollars to have modified and interpreted apply to everyone who learns how to use them. A great foundation book for beginning to improve your financial intelligence so that you don't work 4 or more month's of every year for the Tax man, more months for the banks that hold your mortgage and credit cards, and whatever is left making the company you work for wealthy. Good luck on your journey to being Rich, poor, or middle class.",
           "rating": 4,
           "rating_text": "4.0 out of 5 stars",
           "helpful": "1,186 people found this helpful",
           "comments": null,
           "date": "Reviewed in the United States on June 19, 2017",
           "bage": "Verified Purchase",
           "official_comment_banner": "",
           "url": "https://www.amazon.com/gp/customer-reviews/RIGBUZ8E2S6UT/ref=cm_cr_arp_d_rvw_ttl?ie=UTF8&ASIN=1612680194",
           "img_url": null,
           "variation": "",
           "total_reviews": 65459,
           "overall_rating": 4.7,
           "author_title": "Eugene C.",
           "author_descriptor": "",
           "author_url": "https://www.amazon.com/gp/profile/amzn1.account.AGUEMAJSJVAUZR2OUSFBBNJM3KQQ/ref=cm_cr_arp_d_gw_btm?ie=UTF8",
           "author_profile_img": "https://images-na.ssl-images-amazon.com/images/G/01/x-locale/common/grey-pixel.gif",
           "product_name": "Rich Dad Poor Dad: What the Rich Teach Their Kids About Money That the Poor and Middle Class Do Not!",
           "product_url": "https://www.amazon.com/dp/1612680194"
         }
       ]
     ]
   }
