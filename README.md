# Rails Engine Group

<img src="https://avatars3.githubusercontent.com/u/18108597" width="150" />

这是一个专门编写 Rails 应用常见功能的小组，致力于为快速开发实现各种类型的 Rails Engine Gem，以便我们在做外包，起创业项目的时候，能基于已有的方案快速实现原型，同时又能有良好的可扩展性、可定制性，以便使用者在后期有更多需求的时候，还能基于目前的方案自定义来实现。

### About Rails Engine

> Engines can be considered miniature applications that provide functionality to their host applications. A Rails application is actually just a "supercharged" engine, with the Rails::Application class inheriting a lot of its behavior from Rails::Engine.

http://guides.rubyonrails.org/engines.html


### 什么应该做？ / 不应该做什么？

- 设计好数据库接口；
- 可配置的选项，以便适应更多的项目；
- Generator 生成默认配置信息，可选性的生成 Controller, Views, Helpers, Models 甚至 Assets
- 完整实现的功能，不一定要非常复杂，但得是完善的；
- 应该包含基本的 CSS 样式，以及自己的前端 JS 实现（如果确实需要的话）；
- 支持 ActiveRecord，不要用 PostgreSQL 的特性，以便 MySQL 用户都能用；
- 标准的 Rails Way 实现；
- 在 View 或 CSS 里面用 Bootstrap 作为默认的前端组件, 用 jQuery，不要包含复杂的前端 Framework，比如所见即所得编辑器，这个留给用户自己实现;
- 同上，Views 不一定要非常复杂，这些事情应该留给用户自己实现，因为往往每个项目都有不同的需求；

### 可实现方向

- [用户系统 - Devise](https://github.com/plataformatec/devise)
- [OAuth 服务端 - Doorkeeper](https://github.com/doorkeeper-gem/doorkeeper)
- [论坛系统 - Homeland](https://github.com/rails-engine/homeland)
- [通知中心- Notifications](https://github.com/rails-engine/notifications)
- [私信、站内信 - Innbox](https://github.com/rails-engine/innbox)
- [评论 - comments](https://github.com/rails-engine/comments) - 多态的方式，适合各种类型的场景
- [喜欢、赞、收藏、好友、关注等功能 - actionstore](https://github.com/rails-engine/actionstore) - 多态的方式，适合各种类型的场景
- 动态，Timeline
- 相册
- Page / CMS 用于线上发布独立页面(例如：关于、隐私)，URL 绑定 / 根目录；

### 欢迎参与

如果你有兴趣，可以参考 [notifications](https://github.com/rails-engine/notifications), [homeland](https://github.com/rails-engine/homeland) 的实现方式，选择一个实用的方向做一个新的库。

当然，在你的项目里面使用 rails-engine 里面的库，并给我们反馈或提交改进、Bug 修复也是参与！
