**【GTM】YouBase Launch**

**Goal**

现在的 AI 赛道，“稳步增长”等于“慢性死亡”。我们要的不只是稳扎稳打的线性 User Acquisition，而是指数级的 Hyper-Growth。因此目标不是功能发布，而是 Go Viral。

我们现在的月新增用户是 25 万（PC Web端），如果要达到 **300 万美元 ARR**，我们需要至少 **75 万的 MNU** 才有可能。如果是要达到 **100 万美元的 ARR**，我们也需要至少 **40 万的 MNU**，我们希望通过 YouBase 这次的产品发布来实现潜在的破圈效应。

**Feature Overview (with screen recording)**

PRD：[【YouWare Web】YouBase 1.0](https://kcnz0vt5pezm.feishu.cn/wiki/MPRywD56Li6tRakeXXQcaUfrnKf)

一句话介绍 YouBase：YouBase 是网站/应用的“大脑”、“保险柜”和“收银机”，帮你记住你的用户是谁（登录），也记住他们做了什么（存数据），还能帮你收钱。

|  |
| --- |
| Markdown 咖啡店案例 Prompt： Help me build an online website for Emma’s Coffee Shop.  The homepage should include a hero section and a menu list, and support online ordering. Users are required to log in before placing an order. After logging in, they can place orders, and each order should be linked to the user’s account.  The site should also support an admin account with access to an admin dashboard, where the admin can view order volumes and update order statuses. |

|  |  |  |  |
| --- | --- | --- | --- |
| Feature name | What is this feature used for?   |  | | --- | | 以 Emma 咖啡店线上下单为例介绍 | | Screen recording |
| Database | 数据存储 Data storage   * **菜单管理：**在 Database 里创建了一张“菜单表”，记下：“拿铁 - $5”、“美式 - $3”。想涨价时，改一下这里，网站上所有地方的价格就自动变了。 * **订单记录：**当顾客下单了一杯拿铁，Database 会立刻自动记上一笔：“顾客 A 在 10:05 买了一杯拿铁，未支付”。 * **后台查看：**因为有了数据库，Emma 打开管理员后台时，才能看到今天到底卖了多少钱，哪款咖啡最畅销。 * **Menu management:** A “Menu” table is created in the database to store items like “Latte – $5” and “Americano – $3.” When you want to change the price, you just update it here, and the price is automatically updated everywhere on the website. * **Order records:** When a customer orders a latte, the database immediately records it, for example: “Customer A bought a latte at 10:05, unpaid.” * **Admin dashboard:** With the database in place, Emma can open the admin dashboard to see how much was sold today and which coffee is the best seller. | **[YouBase-database.mp4]** |
| Users & Authentication   * Email Login * Google Login | 用户登录和身份鉴权 User login and authentication  咖啡店需要区分两种人：   * **顾客（会员）：** * **Email / Google Login：** 顾客不需要填繁琐的表格，直接点一下“Google 登录”，就像刷脸进店一样，瞬间拥有了会员身份。 * **作用：** 登录后，系统知道“你是 John”，所以你只能看到 John 的历史订单，看不到别人的。 * **管理员（Emma）：** * **权限控制：** 系统识别出“你是老板 Emma”，所以给你开了“后门”（Admin Dashboard），让你能看到所有人的订单和收入数据。如果没有这个功能，你的商业机密就泄露了。   A coffee shop needs to distinguish between two types of users:   * **Customers (members):** * **Email / Google login:** Customers don’t need to fill out long forms. They can simply click “Sign in with Google”—just like scanning your face to enter a store—and instantly become a member. * **Purpose:** After logging in, the system knows “you are John,” so you can only see John’s order history, not anyone else’s. * **Administrator (Emma):** * **Access control:** The system recognizes “you are the owner, Emma,” and opens a special “back door” (the Admin Dashboard), allowing you to see all orders and revenue data. Without this, your business-sensitive information would be exposed. | **[YouBase-users.mp4]** |
| Storage | 用于存储图片、视频、文件等 Media assets  Used to store media assets such as images, videos, and files   * **展示商品：**拍一张刚刚拉好花的拿铁照片，把它上传到 Storage。 * **自动分发：**当顾客打开网站点单时，YouBase 会从 Storage 里把这张高清大图取出来，展示在顾客的手机上。 * **价值：**只有把照片存放在 Storage 里，无论顾客在美国还是日本，打开菜单，那张拿铁的照片都能瞬间加载出来。 * **Product display:** Take a photo of a freshly made latte with latte art and upload it to Storage. * **Automatic delivery:** When a customer opens the website to place an order, YouBase fetches this high-resolution image from Storage and displays it on the customer’s phone. * **Value:** By storing images in Storage, the latte photo loads instantly when customers open the menu—no matter whether they’re in the US or Japan. |  |
| Secrets | 用于存储敏感信息，比如 API Key  Used to store sensitive information, such as API keys  为了让店铺更高级，你增加了一个 AI 客服机器人（接入 ChatGPT）来回答顾客问题。   * **风险：** 要使用 ChatGPT，需要一个 **API Key**（就像银行卡密码）。如果直接把它写在代码里，就像把银行卡密码贴在店门口，黑客偷走后会刷爆你的卡。 * **YouBase 的作用：**把这个 API Key 放进 YouBase 的 **Secrets** 里。 * **结果：**网站运行时，AI 客服能正常工作（因为后台能悄悄拿到钥匙），但任何访问网站的人（包括黑客）都看不到这把钥匙。你的钱袋子安全了。   To make the coffee shop more advanced, you add an AI customer support bot (powered by ChatGPT) to answer customer questions.   * **Risk:** To use ChatGPT, you need an API key (like a bank card PIN). If you put it directly in the code, it’s like taping your PIN to the shop door—hackers could steal it and rack up charges on your card. * **What YouBase does:** You store the API key securely in YouBase Secrets. * **Result:** When the website runs, the AI customer support works normally (the backend can quietly access the key), but no one visiting the site—including hackers—can see it. Your money stays safe. | **[YouBase-secrets.mp4]** |

**Product Value**

|  |  |
| --- | --- |
| Product Value | How We Did It |
| 便宜/极致性价比  Unbeatable Cost-Efficiency | 对比雇人建站：过往 SMB 的用户 hire freelancer 来帮他们开发网站，需要花几千或上万美金（[详见参考资料](https://kcnz0vt5pezm.feishu.cn/wiki/H1XlwwHBSicK0Hk7UYAcXbgbnAh#share-QC4NddX0WoIALnxg2IucIJarnmf)），但现在 20 美金就可以用 YouWare + YouBase 实现了。  对比其他 AI Coding 竞品：因为技术方案选型的不同，我们的方案成本非常低，我们把 YouBase 打包到了 YouWare 的订阅套餐中，用户在不用额外支付费用的情况下（只需要正常支付YouWare 的订阅费用，如 20 刀/月，即可无限使用 YouBase）。其他竞品针对后端会额外收费，比如 lovable 是需要额外给后端服务（Cloud）充钱的。 |
| 简单易用  Zero-Config, Full-Stack Simplicity | 不需要学习如何配置 Supabase 的 Key、怎么搭建 Shopify 电商网站、怎么使用 WordPress，一句话就可以搭建你的 business 落地页，并且真的可以投入使用并赚到钱。 |
| 全球稳定与企业级安全  Global Stability & Enterprise Security | 基于 xx 架构，YouBase 确保无论用户身处新加坡、纽约还是伦敦，都能获得低延迟和高可用性。我们严格遵守企业级的数据隐私和存储安全标准，解决了用户对 AI 生成代码安全性的信任危机。 |
| 实现可变现的商业闭环  Built for Real Revenue | YouBase 不仅仅存储数据，它可以真的帮你赚钱。通过帮用户连接 Stripe 支付和安全的用户鉴权（Email/Google），用户可以发布功能完善的 SaaS 工具、交易平台或付费会员网站，并在上线第一天就处理真实的交易。 |

**Audience and Key Message**

|  |  |  |
| --- | --- | --- |
| **Audience** | **Pain Point** [**用户声音>**](https://kcnz0vt5pezm.feishu.cn/wiki/H1XlwwHBSicK0Hk7UYAcXbgbnAh#share-BxeDdGCHnoNQiWxzHHDcPckRnHY) | **Key Message** |
| SMB (Small Business Owners) | 没钱雇人，不懂技术，被外包坑过，只想赶紧把生意跑起来收钱。 | 别再花 $5000 雇人写代码了。用 YouWare，一份早餐的钱，一句话生成带支付系统的完整网站，今天上线，今天收钱。 *Don't hire a dev. Build a revenue-generating business with one sentence for $20. Launch today, get paid today.* |
| Prosumer / 想要做副业赚钱的人 (Wannabe Entrepreneurs) | 觉得做网站很贵，学习 WordPress、Verce、Supabase、Shopify 这些工具很难，要花很多时间。 | 你离你的第一个互联网生意，只差一句‘帮我做一个...’。不需要学编程，不需要学 Shopify，我们把技术门槛降到了 0，你只需要负责数钱。 *Your first online business is one prompt away. No coding, no tutorials. We handle the tech; you handle the profit.* |
| 竞品用户 (Users of Lovable, v0, supabase) | 前端写得很爽，一到后端就卡壳，或者被竞品的“Cloud Credits”额外收费刺痛（Hidden Cost） | 还在为 Lovable Cloud 额外付费？YouWare 订阅包含无限后端服务与企业级数据库。同样的 AI 编码体验，我们不收‘云税’。 *Stop paying the 'Cloud Tax'. YouBase gives you unlimited secure backend & storage included in your subscription. Switch to the platform that doesn't punish your growth.* |
| AI 核心圈 / 极客 (Tech Savvy / AI Core) | 质疑 AI 生成的代码无法用于生产环境，担心性能（Latency）和安全性。 | 不只是生成 Demo，而是生成 Production-Ready 的应用。全球节点秒级响应，企业级安全合规。YouBase 是为“真实业务”打造的 AI 基础设施。 *Stop building toys. Build scalable, secure, global-ready applications instantly. Real backend, real business, real fast.* |

**Go-to-Market Strategy**

|  |
| --- |
| **核心策略：**  第一步：通过技术架构、参数、性能表现等体现产品功能强大  第二步：激进对标竞品，心理价格锚定，引发关注  第三步：小米式价格屠夫策略，打极致性价比，限时福利促下单 |

**Slogan**

备选方案：

* YouBase: The World's First AI Co-Founder.
* YouBase: The World's First AI CTO.
* YouBase: The World's First AI Business Engine.
* YouBase: Your First AI Online Business Partner

|  |
| --- |
| 角色化的 Slogan 更让人能共情和记忆：  Lovable: The World's First Al Fullstack Engineer  Manus: The World's First general-purpose Al Agent  Lovart: The World's First Design Agent  Shopify: Your Commerce Platform to Sell Online & In Person |

**Competitor Comparison**

|  |  |  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- | --- | --- |
|  | YouWare + YouBase | Lovable + Cloud（Supabase） | Replit | base44 | No built-in backend AI Coding Platform+SaaS (V0) | Fiverr Freelancer+Cloud Service (like AWS） | WordPress+Plug-in |
| **Backend infrastructure**  后端基础设施 | Built-in | Built-in | Built-in | Built-in | External | External | External |
| **Backend Cost Structure**  后端成本结构 | Free\*  不额外收费 | Usage-based  Compute Instance + Variable Usage (基于用量: 算力实例+可变用量 | Highly Variable Usage-based (Fixed Deployment + Compute Units)  高可变用量: 固定部署费+算力单位 | Opaque Usage-based  不透明的按量计费 | Highly Granular Usage-based (Active CPU Time + GB-Hours)  高度细粒度用量: 活跃CPU时长+内存GB小时 | High Initial Labor + Hidden Operational Costs  高昂初始人工成本+隐藏运维成本 | Fixed Hosting + High Add-on Fees  固定主机费用+高附加组件费用 |
| **Estimated Monthly Base Cost**  月度基础费用估算 | $0\*  包含在 YouWare 的订阅套餐中，无双重计费 | ~$10 (Micro) to ~$110 (Large) for production instances  生产实例最低$10, 大型$110 | Min. ~$41 (Fixed Deployment Base, excluding variable usage)  最低 41/月，不含变量用量 | Custom | ~$20 （Pro Base）+ High Variable Compute Usage  专业层 20/月，高度可变算力用量 | $500 - $5,000+ (Hiring Engineer/Ops)  $500-$5,000+ 雇佣工程师/运维 | $30-$400 |
| **Ease of Use**  易用性 | Easy  自然语言编程 | Easy  自然语言编程 | Medium  自然语言编程，但功能复杂性高 | Easy  自然语言编程 | Medium (Requires integration of external backend service)  自然语言编程，需集成外部后端服务 | Easy (Hiring solution, if requirements are clear) 简单: 雇佣模式, 前提需求清晰 | Hard (Maintenance, plugin conflicts, PHP debugging)  困难: 维护, 插件冲突, PHP调试 |
| **Auto-Scaling/Compute**  服务器算力自动扩容 | Free to scale  免费扩容 | Paid to scale (Instance-based, manual or limited automation)  依赖 Compute 实例升级，当应用需要更高的性能（例如需要专有 CPU 资源）时，必须升级到 Large（$110/月）、XL（$210/月）乃至 4XL（$960/月）的实例 | Paid to scale (Compute unit billing and fixed configuration tiers)  付费扩展: 基于算力单位和固定配置层级 | Paid to scale | Paid to scale(Seamless but high cost volatility)  付费扩展: 无缝但成本波动高 | Paid to scale (Requires manual server upgrade/Ops labor)  付费扩展: 需手动升级服务器/运维成本 | Paid to scale (Plan upgrade based on Visits/Bandwidth)  付费扩展: 基于访问量/带宽升级方案 |
| **Serverless Architecture**  Serverless 架构 | Yes (Integrated Edge Functions)  是: 集成边缘函数 | Yes (Edge Functions available)  是: 边缘函数可用 | Yes (Deployment infrastructure)  是: 部署基础设施 | Yes | Yes (Highly optimized for Edge Functions)  是: 高度优化边缘函数 | No (Traditional VM/container or IaaS)  否: 传统VM/容器或IaaS | No (Monolithic PHP architecture)  否: 单体PHP架构 |
| **Speed/Performance**  全球性能 | Ultra-fast global access (Code deployed closest to user, 300+ nodes)  超快全球化: 代码部署于用户最近节点, 300+节点 | Unstable access speed; Varies by IP/Region  访问速度不稳定; 访问取决于IP/区域 | Varies by deployment type and region  取决于部署类型和区域 |  | Excellent (Global CDN/Edge Functions, low latency)  优秀: 全球CDN/边缘函数, 低延迟 | Dependent on manually selected hosting region  取决于手动选择的托管区域 | Often Slow (Due to PHP processing and plugin bloat)  通常慢: PHP处理和插件冗余 |
| **Agent Friendliness**  Agent 友好度 | High  YouWare 基建原生集成 | High  Lovable 基建原生集成 | High  Replit 基建原生集成 | High  base44 基建原生集成 | Medium (Focus on frontend deployment/tools)  中: 侧重前端部署/工具链 | Not supported | Low (Non-standardized, plugin-dependent environment)  低: 非标准化, 依赖插件的环境 |
| **Security** | Physical Isolation  核心资源与其他用户项目物理分离，提供最高级别的安全和合规保障  *Core resources are physically separated from other user projects, offering the highest level of security and compliance.* | Logical Isolation  资源共享，但通过软件策略隔离，如行级安全策略 (RLS)  *Resources are shared but separated by software policies like Row-Level Security (RLS).* | Logical Isolation  项目在共享资源上运行，依赖内置的Secrets加密和访问控制来区分不同用户的数据。  *Projects run on shared resources, relying on built-in Secrets encryption and access control to separate user data.* | Logical Isolation  使用软件沙箱或容器隔离，而非物理硬件隔离。  *Uses software sandboxing or container isolation, not physical hardware isolation.* | Logical Isolation  使用防火墙和微服务隔离来保护每个函数。这种安全是基于软件沙箱和网络策略的。  *Uses a Firewall and micro-service isolation to protect each function. Security relies on software sandboxing and network policies.* | Logical/Physical Isolation  安全等级取决于你选择的云服务（IaaS/PaaS）和雇佣的工程师的专业度。  *Security depends on the chosen cloud service (IaaS/PaaS) and the expertise of the hired engineer.* | Logical Isolation/Low  依赖插件和运维，缺乏原生安全控制，安全风险高。  *Relies on plugins and maintenance; lacks native security controls, leading to high security risk.* |

**Beta release**

**Actions**

|  |  |
| --- | --- |
| **渠道 (Channel)** | **动作 (Action)** |
| X/Linkedin official | [YouBase Launch Marketing Cadence](https://kcnz0vt5pezm.feishu.cn/wiki/J5LXwYp6Jinp5OkmMKKcSR0cnve) |
| Contra 联名黑客松  Contra Hackathon Partnership |
| EDM | 全员邮件通知 YouBase Beta 上线，同时宣传 X 上的免费赠送 credits 的活动，邀请用户参与 @Keira |

**Assets**

**Promotional Video 宣传片**

|  |  |  |
| --- | --- | --- |
| Video Type | Script | Video |
| 15s YouBase Beta release video | [15s YouBase Beta Launch Script](https://kcnz0vt5pezm.feishu.cn/wiki/GzYBwfJg4i9PchknwrNcvXBCnSg) | **[YouBase 短视频(5).mp4]**  **[YouBase 短视频(5).zip]** |
|  |  |  |

**Key Selling Points Poster 卖点海报**

|  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- |
| **宣传点 Selling Points** | 优先级 | DDL | 设计交付稿 Deliverables | **物料 Key Assets** | **参考内容 Reference** |
| **Unbeatable Cost-Efficiency**   1. **Compared to hiring freelancers:** 不用支付高昂的人力成本 Avoid high labor costs 2. **Compared to Supabase, Vercel, AWS:** 后端服务价格昂贵 Backend services come with high bills | P0 | 12.17 | ![](data:image/png;base64...)  ![](data:image/png;base64...)  ![](data:image/png;base64...)  ![](data:image/png;base64...) | 1. **Fiverr 避坑指南 (The Fiverr Roast)**  * **视觉描述 (Visual):** * **背景：** 直接使用真实 Fiverr 吐槽截图（比如那个花了 $3000 没拿到源码的），对 Fiverr 的 Logo 进行模糊处理。Use real Fiverr complaint screenshots directly * **前景：** 打上一个鲜红的 **"AVOID THIS"** 印章。Add a bold red “AVOID THIS” stamp * **文案 (Copy):** * **Headline:** $3,000 & 4 Weeks?! * **底部横幅：**YouBase by YouWare: Zero risk, own your code, all for $20/mo.  1. **账单粉碎机 (The Invoice Crusher) - TBD (suggest using video format)** 2. **视觉描述 (Visual)**  * 左边：Supabase 账单，Vercel 账单，AWS 账单 拼贴在一起，价格放大 **Left:** Stacked Supabase, Vercel, and AWS bills with exaggerated prices. * 右边：只有 YouWare 的 Logo 和一句 Prompt。底部价格用巨大的绿色字体标出：Included for $20/mo. **Right:** Clean YouWare logo with one simple prompt. Bold green text at the bottom reads Included for $20/mo. * 动作感：中间有一条撕裂线，或者右边的画面正在“挤压/粉碎”左边的画面。A dramatic tear or crushing effect where the YouWare side overwhelms the bills.  1. **文案 (Copy):**  * **Headline:** Get $2,000 of product value for $20. * **Body:** We're crushing the cost of cloud infrastructure for you. Keep more of your profit with YouBase.  1. **Tech Blog：**详细解释 YouBase 如何通过技术优化压低成本 A detailed explanation of how YouBase optimizes costs through technical innovations | 1. Fivver roast   ![](data:image/png;base64...)  https://www.reddit.com/r/legaladvice/comments/1papp7r/fiverr\_dev\_took\_3000\_project\_incomplete\_access/   1. Receipt  |  |  | | --- | --- | | ![](data:image/jpeg;base64...) | ![](data:image/jpeg;base64...) |  |  |  | | --- | --- | | ![](data:image/png;base64...) | ![](data:image/png;base64...) | |
| **Transparent**   1. **Compared to Lovable, Replit:**  * 竞品的后端服务需要单独计费 Competitors' backend services require separate billing * 竞品的后端计费根据不同模块的用量计算 Competitors charge backend usage based on individual modules | P0 | 12.16 | ![](data:image/png;base64...) | 1. **账单解剖图（Billing breakdown diagram）** 2. **视觉描述 (Visual):** 3. 左边（红色）：画一个复杂的冰山。最上面写着“Subscription”，剥开一层是“Compute Credits”，再剥开是“Bandwidth Fees”，再剥开是“Storage Overages”。   Illustrate a complex iceberg. At the very top, label it “Subscription.” Peel back one layer to reveal “Compute Credits,”then another layer showing “Bandwidth Fees,”and another revealing “Storage Overages.”   1. 右边（绿色）：一个干净的实心方块。写着：“YouBase by YouWare: Everything Included in Subscription.”。Next to it, show a clean, solid block labeled: “YouBase by YouWare: Everything Included in Subscription.” 2. **文案 (Copy):** 3. **Headline:** You're done paying "Cloud Tax" and hidden fees. 4. **Sub:** Stop paying double. One YouBase plan comes with an unlimited backend. | ![](data:image/png;base64...)  Nano banana 画的参考图 |
| **Auto-Scaling/Compute**   * **Your fees won’t increase significantly as you scale：**竞品的用户项目规模越大成本越贵 Competitors' backend services costs **increase significantly** as your usage scales | P1 |  | ![](data:image/png;base64...) | 1. **成本规模曲线图（Cost–Scale Curve）** 2. **视觉描述 (Visual):**  * 横坐标轴规模、纵坐标轴 Cost 的曲线图 Cost curve chart (X-axis: You scale, Y-axis: Your cost) * Replit 随着用户规模增大，成本快速增长，YouWare 随着规模增长成本涨的很缓慢，lovable 介于二者之间 Replit’s costs increase rapidly as user scale grows, YouWare’s costs rise much more slowly, and Lovable falls somewhere in between.  1. **文案 (Copy):**  * **Headline:** Grow 10x. Pay 1x.*(增长 10 倍。付费 1 倍。)* * **Sub-text:** Don't go auto-bankrupt trying to auto-scale. Keep your margins with YouBase.*(自动扩容不该意味着自动破产。在扩张时守住你的利润。)* | ![](data:image/png;base64...)  参考这张图，但是我们的坐标不同 |
| **Speed/Performance**   * YouWare's ultra-fast global access (Code deployed closest to user, 300+ nodes) YouWare 超快全球化，代码部署于用户最近节点, 300+节点 * Competitors' unstable access speed; Varies by IP/Region 竞品的访问速度不稳定，访问取决于IP/区域 | P1 |  | ![](data:image/png;base64...) | 1. **全球访问速度图 “点亮地球”（Global access speed map with a “Light Up the Globe” effect）** 2. **视觉描述 (Visual):** 3. 一张深色的 3D 地球背景。在世界主要城市（纽约、伦敦、新加坡、东京、悉尼）同时亮起绿色的光点。 A dark 3D Earth background. Green light points illuminate simultaneously over major global cities, including New York, London, Singapore, Tokyo, and Sydney. 4. 每个光点旁边标注极低的 Ping 值（如 "45ms", "30ms"）。Each light point is labeled with an ultra-low ping value, such as “45ms” or “30ms.” 5. **文案 (Copy):**  * **Headline:** Reliable Global Network. * **Sub:** Whether you are in San Francisco or Singapore, your app will load instantly. | Cloudflare 的网络地图： [Cloudflare Network Map](https://www.google.com/url?sa=E&q=https%3A%2F%2Fwww.cloudflare.com%2Fnetwork%2F) (这种发光的地球是展示速度的标准答案，非常有科技感)  ![](data:image/png;base64...) |
| **Easy to use**   * Don’t need to learn complex tutorials or figure out how to configure API keys. With YouWare, natural-language instructions are all you need — simple and effortless. | P0 |  | **[20251223174715\_rec\_-convert.mp4]** | 1. **V0 和 YouWare 的对比录屏** Screen recording comparing V0 and YouWare ✅ 2. **后端开发进化论（The Evolution of Backend Development）**  * **视觉描述 (Visual):** * 左边：一张密密麻麻的 SQL 代码截图 + 复杂的 API 配置文档截图。A dense SQL code screenshot plus a complex API configuration document screenshot. Labeled: "The hard way"。 * 中间：一个箭头。An arrow. * 右边：一个聊天气泡，A chat bubble.里面写着："Create a waitlist page to collect emails." 标注："The easy way (with YouBase)"。   A chat bubble with the text: "Create a waitlist page to collect emails." Labeled: "The easy way (with YouBase)"   * **文案 (Copy):** * **Headline:** English is the new SQL. * **Sub:** Tell YouBase's AI what you need. Backend is built-in.  1. **YouBase 的 Prompt 技巧 Blog** | 1. 后端开发进化论（The Evolution of Backend Development）  |  |  | | --- | --- | | ![](data:image/png;base64...)  GPT | ![](data:image/png;base64...)  Nano banana |  1. Prompt Blog   https://x.com/damienghader/status/1998776888718942589?s=20  ![](data:image/png;base64...) |
| **Security**   * Encrypt data：一些竞品会在前端代码里暴露用户的敏感信息如 API KEY，不安全，而 YouWare 的 secrets 功能可以保护这些敏感信息不被泄露 Some competitors expose users’ sensitive information—such as API keys—in the frontend code, which is insecure. With YouWare’s Secrets feature, this sensitive data is fully protected and never exposed. * 物理隔离 vs 逻辑隔离 Core resources are physically separated from other user projects, offering the highest level of security and compliance. * Auth 功能里的邮箱登录，可以开启邮箱验证，防止恶意注册，防止用户账号被盗用 Email login supports optional email verification to reduce malicious registrations and prevent account abuse. | P1 |  | ![](data:image/png;base64...)  ![](data:image/png;base64...) | 1. **保险柜与防盗门（Vault and Security Door）** 2. **主体布局：** 将整个海报分为 3 个并列的卡片区域。每个区域代表一个安全维度。Divide the poster into three side-by-side card sections. Each section represents a security dimension.  * **区域 1: 数据加密 (Encrypted)** * **画面:** 一个发光的**数据块**或**硬盘图标**，周围有旋转的**加密锁链**或**二进制代码流**。核心元素是一个**紧锁的锁头图标 🔒**。**A glowing data block or hard drive icon**, surrounded by rotating encrypted chains or flowing binary code. The core element is a **locked padlock icon** 🔒. * **文案 (Copy)：** * Data Safety * Keep your data encrypted to protect it from anyone but you. * **区域 2: 隔离防护 (Isolated)** * **画面:** 多个**透明的应用模块（小方块）**，它们之间有清晰的“防火墙”**或**“隔离带”线条。每个模块中间有 YouBase 的小 Logo。核心元素是一个“物理隔离墙”或“屏障”图标 🧱。**Multiple translucent application modules** (small square blocks) with clear **“firewall” or “isolation barrier”** lines between them. Each module contains a small **YouBase logo** at its center. The core element is a **“physical isolation wall” or “barrier”** icon 🧱. * **文案 (Copy)：** * Isolate your Environment * With YouBase, your projects will run in a secure, dedicated space. * **区域 3: 用户验证 (Verified Users)** * **画面:** 一个带有 **Google 登录按钮**和 **Email 输入框**的简洁登录界面截图（类似 Clerk 截图右上角的风格）。**核心元素是**一个**绿色的打勾图标 ✅**，旁边写着 Email Verified。**A clean login interface screenshot** featuring a **Google sign-in button** and an **Email input field**. The core element is a **green checkmark icon** ✅ with the text **“Email Verified”** beside it. * **文案 (Copy)：** * Protect with User Verification * Let who you want in. Block the bots and fraud out.  1. **文案 (Copy):** 2. **Headline:** **Security. Built-in. Always On.** 3. **Sub:** Enterprise-grade protection, so you can focus on building. 4. Tech blog | ![](data:image/png;base64...)  https://clerk.com/ |
| **Production ready** | P0 |  | ![](data:image/png;base64...) | |  | | --- | | **There are two visual design options to choose from.** |  * **方案一：玩具车 vs 赛车（Toy Car vs Race Car）** * **视觉描述 (Visual):** * 左边：一个乐高拼的玩具车，标注 "Other AI Builders (Prototypes)"。 * 右边：一辆特斯拉或 F1 赛车（代表 YouBase），车身上印着 Database, Auth 的 Logo，标注 "YouBase (Real Business)"。 * A LEGO-built toy car next to a Tesla or an F1 race car. * **文案 (Copy):** * **Headline:** Stop Building Toys. Start Building Businesses. * **Sub:** Don't let your idea die in the "Demo" phase. Scale with a real backend. * **方案二：架构透视 (The Architecture Layers)** * **视觉描述 (Visual):** * **左边 (Competitors):** 一张悬浮的、薄薄的 UI 界面（比如一个简单的网页截图），下面空无一物，或者只有几根断裂的电线。**标注：** **"Just UI / Mockup"**。   A floating, thin UI layer (for example, a simple webpage screenshot) with nothing underneath, or only a few broken wires.   * **右边 (YouBase):** 同样的 UI 界面，但它下面连接着厚厚的、坚实的“技术地基”。这个地基是半透明的 3D 模块，里面发光显示着 **Database** (圆柱体), **Auth** (盾牌), **Storage** (云)。**标注："Full Stack Business"**。   The same UI, but this time connected to a thick, solid technical foundation beneath it.   * **文案 (Copy):** * **Headline:** Give Your Business a Real Engine * **Sub-text:** Competitors give you a frontend shell. We give you the backend engine to actually run it. | Nano banana 画的参考图   |  |  | | --- | --- | | ![](data:image/png;base64...) | ![](data:image/png;base64...) |   ![](data:image/png;base64...) |
| **Cloudflare Partnership** | P1 |  |  |  |  |

**Feature Poster 功能海报（5+1）**

|  |  |  |  |  |  |
| --- | --- | --- | --- | --- | --- |
| 功能 | 优先级 | DDL | 设计交付稿 Deliverables | 物料 Key Assets | 参考内容 Reference |
| **YouBase** | P1 |  |  | **Bento 图** |  |
| **Database** | P0 | 12.16 | ![](data:image/png;base64...) | * **视觉画面：** YouBase 数据库表格界面的特写（Dark Mode）。高亮显示“Schema”结构，展示数据行。旁边浮现几个浮窗图标：JSON, SQL, CSV，暗示支持多种格式。在界面的右上角，高亮一个点击状态的按钮 **"Export"**。从这个按钮中，漂浮出发光的 3D 文件图标：SQL、CSV。它们呈现飞出的姿态，暗示数据可以自由流向外部。   Close-up of the YouBase database table interface (Dark Mode). The Schema structure is highlighted, with data rows visible. Several floating overlay icons appear nearby — JSON, SQL, CSV — hinting at support for multiple formats. In the top-right corner of the interface, a highlighted “Export” button is shown in a clicked state. From this button, glowing 3D file icons labeled SQL and CSV float outward, suggesting that data can freely flow outside the system.   * **文案：** * **Headline:** Your Data. Organized & Yours. * **Feature:** Instant Table Setup. Zero Config. 100% Exportable. | ![](data:image/png;base64...)  https://supabase.com/database |
| **Time Travel**   * database auto backup 备份，不用担心数据库出错 * Enter a time to restore your database to that exact historical point. | P1 |  | **[youbase-feature-timetravel.mp4]**  ![](data:image/png;base64...) | * **视觉画面 (Visual):** * **主体：** 一个发光的时钟或雷达扫描图，中心是 YouBase 的数据库图标。A glowing clock or radar scan graphic, with the YouBase database icon at the center. * **数据流：** 周围环绕着代码或数据流，正在从“模糊/删除状态”重组为“清晰状态”。Code or data streams swirl around it, transforming from a blurred or erased state into a clear, restored state. * **信任标：** 右下角加一个盾牌图标：Auto-Backup Enabled。Add a shield icon in the bottom-right corner labeled “Auto-Backup Enabled.” * **文案 (Copy):** * **Headline:** Time Travel is Real. *(时光旅行是真的。)* * **Feature:** Accidental delete? No problem. Go back in time and save your data.*(误删了？没问题。穿越回过去，救回你的数据。)* | Nano banana 画的参考图  ![](data:image/png;base64...) |
| **Auth**   * 实现注册和登录功能 * 查看 user dashboard 仪表盘 | P0 | 12.16 | ![](data:image/png;base64...) | * **视觉画面：** * 左上角：一个精美的登录框 UI（Google 按钮 + Email 输入框）。A polished login UI with a Google sign-in button and an email input field. * 右下角：User Dashboard 的数据图表（展示 User Growth 曲线）。A User Dashboard with data charts showing user growth trends. * **关键点：** 要有一个盾牌小图标打在 Email 输入框旁，标注 "Verified Only"。A small shield icon next to the email input field, labeled “Verified Only.” * **文案：** * **Headline:** Turn Visitors Into Users * **Feature:** Secure Login, Email Verification, & User Dashboard included. | https://x.com/supabase/status/1996682228307292367?s=20  ![](data:image/png;base64...) |
| **Storage** | P0 | 12.16 | ![](data:image/png;base64...) | * **视觉画面：** 一个云端文件夹的 3D 渲染图。文件像卡片一样飞入文件夹中。展示图片、PDF、视频图标。A 3D-rendered cloud folder. Files fly into the folder like cards, showing image, PDF, and video icons. * **文案：** * **Headline:** Store Anything. Scale Anywhere. * **Feature:** Seamless file uploads for your users. Images, videos, docs. | ![](data:image/png;base64...)  https://vercel.com/storage/blob |
| **Secrets** | P0 | 12.16 | **[youbase-feature-secret.mp4]**  ![](data:image/png;base64...) | * **视觉画面：**一个加密的保险箱 UI。An encrypted vault UI. * 显示 Key 的名称（如 STRIPE\_SECRET\_KEY），但 Value 显示为 ••••••••••••（隐藏状态）。The key name is visible (for example, STRIPE\_SECRET\_KEY), while the value is hidden and shown as ••••••••••••. * **文案：** * **Headline:** Keep Secrets, Secret. * **Feature:** Never expose your API keys. Server-side environment variables protection. | |  |  | | --- | --- | | ![](data:image/png;base64...) | ![](data:image/png;base64...) |   https://www.doppler.com/solutions/use-cases/single-source-of-truth |
| **实时后端调试 Log**  Real-time backend debug logs | P1 |  | **[youbase-feature-log.mp4]**  ![](data:image/png;base64...) | * **视觉画面：** * 类似黑客帝国的“代码雨”或者终端（Terminal）界面，黑底绿字/白字。A Matrix-style “code rain” or terminal interface. Black background with green or white text. * 高亮一行字：[SUCCESS] Payment Intent Created - 200 OK。 * 旁边放一个“实时（Real-time）”的脉冲图标。A “Real-time” pulse icon displayed alongside. * **文案：** * **Headline:** Full Visibility. In Real-Time. * **Feature:** Watch your backend logic run live. Debug instantly. No black boxes. | |  |  | | --- | --- | | ![](data:image/png;base64...) | ![](data:image/png;base64...) |   https://vercel.com/docs/logs/runtime  Nano banana 作品  ![](data:image/png;base64...) |

**Official release**

|  |  |
| --- | --- |
| **渠道 (Channel)** | **动作 (Action)** |
| X/Linkedin official | [YouBase (Official) Launch Marketing Cadence JAN](https://kcnz0vt5pezm.feishu.cn/wiki/ZqkBwTolIick5RkjvgccYg4PnFf?from=from_copylink) |
| Cloudflare Co-branding: Tech Blog |
| Social Media Challenge | [YouBase Launch Campaign](https://kcnz0vt5pezm.feishu.cn/wiki/MeB6wMqUIinnElkWdMecNo3xn5d) |
| EDM | @Keira |
| KOL | @Shelley |
| SEO | https://www.youware.com/features/youbase |

**Timeline**

![](data:image/png;base64...)

**Click the image to view the bitable.**

**References**

**User Pain Point**

All 👉[lovable/.../用户 cloud 吐槽](https://kcnz0vt5pezm.feishu.cn/docx/SU9WdrNT8ontnQxHi93c5awmnKd)

|  |  |  |
| --- | --- | --- |
| User Group | User Voice |  |
| SMB & Prosumer | ![](data:image/png;base64...)  https://www.reddit.com/r/legaladvice/comments/1papp7r/fiverr\_dev\_took\_3000\_project\_incomplete\_access/ | 用户在 Fiverr 花 3000 美元分阶段找人做定制网站，但过程拖延、只给演示视频不交真实权限，作为非技术人员当时难以验收。后来请了新开发接手才发现：数据库导出无效、密钥/访问权限没交接、部署不在自己控制下，很多地方几乎需要重做。  现在 Fiverr 说“技术上已交付且过了取消窗口”，只愿意退约 50%，用户想问：要不要接受这 50% 退款，还是继续争取全额退款（地点在美国华盛顿州）。 |
| ![](data:image/png;base64...)  https://mashable.com/article/upwork-scam-safety | 我在 Upwork 上被骗了，这样你就不用再被骗了，我在零工经济剥削中的 475 美元教训 |
| ![](data:image/png;base64...)  https://www.reddit.com/r/ecommerce/comments/18bvu7w/im\_scared\_to\_pull\_the\_trigger\_on\_a\_5k\_website/ | 用户之前在 Fiverr 花了约 2k 找开发但效果很差；现在联系到一家口碑不错的机构报价 5k 做定制站，作品他很喜欢。虽然有钱付，但担心再失败就投入到 7k、压力太大，所以发帖求大家给他“推一把”让他下决心（也提到考虑用 Shopify）。 |
| Competitor users | ![](data:image/png;base64...)  https://www.reddit.com/r/replit/comments/1gwusdt/replit\_insane\_pricing/ | 用户吐槽 Replit 定价“越来越离谱”：以前基本免费、好用，还买过 Core 会员；现在感觉会员也不值，AI 和很多功能都要额外付费。数据库与存储计费也变贵，按计算小时/存储收费，24/7 跑起来一个月可能飙到几百美元，让他一直担心账单、体验变差。 |
| ![](data:image/png;base64...)  https://community.vercel.com/t/v0-issues-with-user-authentication-and-json/8213 | 用户是非技术新手，用 v0 做 app（后端用 Neon），但遇到一堆“认证/部署”相关问题：登录不持久、头像上传后下次登录丢失、用户提交内容保存失败且报认证错误、认证状态按钮判断不准；同时部署到 Vercel 还报动态路由 slug 冲突，v0 修复也无效。后来用 Gemini 排查认为：v0 预览/沙盒环境可能和 jsonwebtoken v9 不兼容，导致服务端路由导入 jwt 就崩溃，直接 500，代码还没跑就挂了。 |
| ![](data:image/png;base64...)  https://www.reddit.com/r/boltnewbuilders/comments/1p1icpm/deployment\_issues/ | 用户在 bolt（以前用 base44）做了一个全栈应用，想用 bolt 自带的数据库/托管，但到部署时怎么都跑不起来，改了很多次连 AI 和 ChatGPT 也解决不了。 |
| ![](data:image/png;base64...)  https://www.reddit.com/r/lovable/comments/1nh7ebz/stop\_using\_lovable\_with\_supabase\_it\_can\_leak\_your/ | 用户警告：Lovable 搭配 Supabase 可能会把数据库访问密钥暴露在前端代码里，导致别人很容易拿到 key、公开访问/泄露整个数据库。他自己检查网页源码也看到了 key（提示用浏览器 inspect element 搜 eyj 之类），想问官方有没有在修复。 |
| AI KOL | ![](data:image/png;base64...)  https://x.com/ballava\_/status/1995739323602464847 | Vibe Coding 只是个玩具 |
| ![](data:image/png;base64...)  https://www.linkedin.com/posts/rodfernand\_most-people-think-vibe-coding-can-ship-activity-7395798709726515200-g8my/ | AI 只能做 demo，而不是产品。 |

**YouWare Use Cases**

|  |  |  |  |
| --- | --- | --- | --- |
| Scenario | Industry | Use Cases | 后端功能需求说明 |
| Website | 教育 | [Dion](https://kcnz0vt5pezm.feishu.cn/wiki/IjlzwgTM9iJaqkkt7DmcgdUBnUe?from=space_search)：教育技术会议官方网站 | 多学校登录系统、数据分析报告、管理员账户、用户使用量控制 |
| [Richard Velez](https://www.youware.com/profile/12LGa5VyK5gSuIZC8cKtM5ULJpY2)：在线教育平台提供课程资源 | 进度追踪记录、实时评分的互动测验系统以及 pdf 证书生成，可以用 storage 存储相应的学习资源 |
| [Hope Seidman](https://kcnz0vt5pezm.feishu.cn/wiki/PaURw6CcCisMi7k4Coxchjxxnnd?from=space_search)：perspectivology AI 专家网站 | 动态数据展示、表单收集 |
| Web3 | [Ihab Salloum](https://kcnz0vt5pezm.feishu.cn/wiki/SuBAwU7C3iPgdCkaOOGcIGg4nub?from=space_search)：投资服务引流网站、加密货币交易分析工具 | 客户注册、订阅周期管理、行情数据API、数据分析 |
| [Crypto Yield](https://www.youware.com/profile/a28z3gAV1pOQ2p03wlSnKHhgSOV2)：区块链投资平台，提供每日返利和自动化收益功能 | 数据库记录用户、投资、交易、钱包以及设定定时任务（网站程序性每日自动返利、抽奖、备份），以及交易、存款凭证图片上传与管理 |
| 电商 | [Christina](https://kcnz0vt5pezm.feishu.cn/wiki/UMufwfSf6i8C5gki4c1cRpTcnPh?from=space_search)：Forever Still Beauty 护肤品牌网站 | 支付集成(Stripe)、会员订阅、联盟营销追踪 |
| 本地生活 | [Newton](https://kcnz0vt5pezm.feishu.cn/wiki/Chc6wOdkbianCVkujDRcybuKnXc?from=space_search)：本地餐厅/夜生活导航网站 | 商家数据库、用户账户登录、商家付费后台、广告位管理 |
| Internal Tools | SaaS | [Tracy Williams](https://kcnz0vt5pezm.feishu.cn/wiki/OX9mwdLZKirHcwkKnfHc0PDGncf?from=space_search)：植物店后台管理系统 | 客户预约系统、客户信息数据库、AI客服机器人、服务记录管理 |
| [Rondinely passos](https://www.youware.com/profile/20Pm39JyDjUEc5QE8FJzKdYKw1N2)：巴西汽车经销商管理系统 | 集成 n8n 工作流自动化和 WhatsApp 进行语音文字交互、媒体存储车辆照片、视频、检测报告、催收系统（催款） |
| 医疗 | [Luciano Rodrigues](https://kcnz0vt5pezm.feishu.cn/wiki/LNXswpaHliAL9QkcpR8cv3M5n7g?from=space_search)：物理治疗师，患者档案管理系统 | 患者信息数据库、诊所管理后台、登录系统、AI辅助诊断 |
| Application for Sale | AI Tool | [suhail](https://kcnz0vt5pezm.feishu.cn/wiki/UOUwwxhZ7i0iQYkLOCdcpHEgntg?from=space_search)：AI电子收据生成器、AI健康与营养跟踪平台 | 数据库、用户认证注册、付费订阅系统、支付集成 |
| [Khayan Lewis](https://kcnz0vt5pezm.feishu.cn/wiki/F2Iew1oCUimqJfkleHwcMp1kn4d?from=space_search)：AI Avatar Studio | 图片存储画廊、用户付费使用功能 |

**Website Building Cost**

|  |
| --- |
| https://www.fiverr.com/resources/guides/business/cost-to-build-website |

**Small business websites:** Costs range from $500 to $5,000, depending on the complexity of the design and features required.

**E-commerce sites**: Prices range from $2,000 to $10,000, influenced by the number of products, payment gateways, and additional features like customer accounts.

**Corporate websites**: Large-scale sites with custom designs, integrations, and advanced functions can cost from $10,000 to $50,000.

![](data:image/png;base64...)

**Click the image to view the sheet.**

**Competitor Pricing**

**Hire a freelancer:**

[Fiverr & upwork](https://kcnz0vt5pezm.feishu.cn/docx/AINldD3wpobsESx4pa8c9FxKnAh)

**Price Range:**

On Fiverr, simple landing pages or single-page websites start at **$80–$90**, while multi-page custom or e-commerce websites in the examples above range from **$250 to $490**.

**Deliverables:**

Basic packages typically include **one page, responsive design, and a limited number of plugins/extensions**, but **exclude payment or marketing integrations**. Standard packages add **more pages and plugins/extensions**, while advanced packages include **e-commerce capabilities, payment integration, subscription forms, and performance optimization**.

**Upwork vs. Fiverr Comparison:**

Upwork project examples show a similar tiered structure, with **$95 for a basic landing page**, **$300 for a four-page site**, and **$600 for an advanced eight-page site with e-commerce functionality**.

**Website builder pricing (Lovable/Replit/WordPress/Shopify/Wix)**

[建站工具对比（简化版）](https://kcnz0vt5pezm.feishu.cn/docx/HrZSdLvFaot9A3xiEMOcFlp2nn4)

**脑暴**

未来是不是可以让用户把其他平台的数据迁移到 YouBase？

https://x.com/supabase/status/1997705182369526204?s=20

![](data:image/png;base64...)

<https://x.com/felixhhaas/status/1996930891411870063?s=20>

![](data:image/png;base64...)