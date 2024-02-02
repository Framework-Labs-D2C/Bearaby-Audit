## Lighthouse speed reports

| id | created\_at | shop | theme\_id | url  | home\_mobile | product\_mobile | collection\_mobile | home\_desktop | product\_desktop | collection\_desktop |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| z6z6hm | 2024-02-01 15:25:59.909 | bearabystore.myshopify.com | 135310999738 | https://bearabystore.myshopify.com/products/the-napper?desktop  | 33 | 30 | 33 | 74 | 51 | 56 |
| k1scwl | 2024-02-01 15:25:06.039 | bearabystore.myshopify.com | 135310999738 | https://bearabystore.myshopify.com/products/the-napper?desktop  | 34 | 28 | 33 | 74 | 62 | 72 |
| ajtzyd | 2024-02-01 15:24:34.866 | bearabystore.myshopify.com | 135310999738 | https://bearabystore.myshopify.com/products/the-napper?desktop  | 34 | 28 | 32 | 75 | 57 | 72 |
| fc1iwh | 2024-02-01 15:21:38.892 | bearabystore.myshopify.com | 135310999738 | https://bearabystore.myshopify.com/products/the-napper?preview\_theme\_id=135310999738&desktop  | 32 | 27 | 28 | 61 | 48 | 62 |

The biggest issue is that a performance script is active (similar to our Performance App, but it runs client side only, which kind of gives the worst effect, which is a delayed user experience start, and still a very high initial page load. The only benefit is that compute time is delayed.)
This also blocks some of the testing options for server rendered performance.

A major issue is that no Image optimization is happening. All images are loaded in only 1 fixed size and not dynamically based on the users screen size.


(Note to future dev / design task) There is a ton of customizations around the Product integrating Weights / Sizes


The Cart Drawer (Add to Cart Actions) is very slow with regard to updates, making 5 rounds of API request that could be handled by a single API request to the cart api.

There are a couple of uniquely designed sections, that look great, but have a very low usability, i.e. buttons that are way to small to click / poorly implemented mobile designs.
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/d77bd67c-c1ca-403b-9854-5593e07aba04)

Lots of unused JS being loaded into the site:
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/dd2f48d5-11b1-4acf-a3ff-7cb3b74a45f7)

Blocking JS time - 5s on mobile is very long
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/20e8268a-5edd-4054-bf14-76093e13f445)

Server side performance is good to very good. Only the Products-slider isn't well optimized.
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/556832d8-0067-422e-9cca-cf9f020fd147)


## Actual Conversion Rates over time:

![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/4828161c-bf31-4da8-8e3f-dc33af32a9b2)

![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/ecbaedbe-125e-449a-853a-bb369918ab36)
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/3ac0f34f-0dac-427f-a8db-fc89d2f50c0c)
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/021c629a-6f77-4b63-b85d-761acbbf20a3)
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/caca1fdb-fd38-4193-99fc-e7b50bb3390a)
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/781477ac-a308-4cd7-920a-18e0c08f839a)
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/c4861ec2-d9bd-42e9-92e4-7afe7ae8cffa)
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/3466c11d-ffe5-40a9-a923-b0d278078fa3)
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/6ad07c59-4303-4daf-9ed5-8f5e5d5ab08b)
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/ab34144c-816f-4278-a195-865f7a3845cc)
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/2a47b643-0b68-4641-892a-09d45afd4f3d)
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/0168ea13-4b9b-4660-b812-eb6c8aa8a499)
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/b3724570-5760-449d-a63d-579ac50556f2)
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/b6b562ca-66d3-4b18-a320-744c6cf83022)
![image](https://github.com/Framework-Labs-D2C/Accelerate-Bearaby/assets/22034038/c192af68-b976-4069-9259-1ce86632b810)



