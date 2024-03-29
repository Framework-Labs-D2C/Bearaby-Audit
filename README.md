## Technical Audit

| id | created\_at | shop | theme\_id | url  | home\_mobile | product\_mobile | collection\_mobile | home\_desktop | product\_desktop | collection\_desktop |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| z6z6hm | 2024-02-01 15:25:59.909 | bearabystore.myshopify.com | 135310999738 | https://bearabystore.myshopify.com/products/the-napper?desktop  | 33 | 30 | 33 | 74 | 51 | 56 |
| k1scwl | 2024-02-01 15:25:06.039 | bearabystore.myshopify.com | 135310999738 | https://bearabystore.myshopify.com/products/the-napper?desktop  | 34 | 28 | 33 | 74 | 62 | 72 |
| ajtzyd | 2024-02-01 15:24:34.866 | bearabystore.myshopify.com | 135310999738 | https://bearabystore.myshopify.com/products/the-napper?desktop  | 34 | 28 | 32 | 75 | 57 | 72 |
| fc1iwh | 2024-02-01 15:21:38.892 | bearabystore.myshopify.com | 135310999738 | https://bearabystore.myshopify.com/products/the-napper?preview\_theme\_id=135310999738&desktop  | 32 | 27 | 28 | 61 | 48 | 62 |

There does not seem to be any image optimization occurring. All images are loaded in only 1 fixed size and not dynamically based on the users screen size.

There seems to be a performance script that is active, similar to Platter's performance app, but Bearaby's runs client side only. This results in a delayed user experience to start, without deferring the very high initial page load. The only benefit is that compute time is delayed. The script also blocks some of the testing options for server rendered performance.

Note to future dev / design task, there is a ton of customizations around the Product integrating Weights / Sizes

The Cart Drawer (Add to Cart Actions) is very slow with regard to updates, making 5 rounds of API request that could be handled by a single API request to the cart api.

There are a couple of uniquely designed sections, that look great, but have a very low usability, i.e. buttons that are too small to click.
![image](https://github.com/Framework-Labs-D2C/Bearaby-Audit/blob/main/bearaby-1.png)

Lots of unused JS being loaded into the site:
![image](https://github.com/Framework-Labs-D2C/Bearaby-Audit/blob/main/bearaby-2.png)

Blocking JS time - 5s on mobile is very long
![image](https://github.com/Framework-Labs-D2C/Bearaby-Audit/blob/main/bearaby-3.png)

Server side performance very good. Only the products slider isn't well optimized.
![image](https://github.com/Framework-Labs-D2C/Bearaby-Audit/blob/main/bearaby-4.png)


## Usability Audit

The 'Quick Add' button doesn't work on mobile. 

https://drive.google.com/file/d/1QjIqtiuKT4jRoJpyr7wD28Iptlx-pn7b/view?usp=sharing
