
## Introduction
This project is a beautiful dashboard based on [Laravel](https://laravel.com/), [vue](https://github.com/vuejs/vue) and use the UI Toolkit [element](https://github.com/ElemeFE/element).

This Laravel-Vue project is inspired by the awesome [vue-element-admin](http://panjiachen.github.io/vue-element-admin) (many thanks to [PanJiaChen](https://github.com/PanJiaChen) for the great works). Newest development stack of Laravel/Vue such as i18n, Envoy, vue-router,.. will be applied into this project.

## DEMO
![](https://user-images.githubusercontent.com/39370721/53298696-afcdae00-3842-11e9-876c-418656c18130.gif)

## Preparation
** [Node](http://nodejs.org/)

** [Git](https://git-scm.com/)

** [Laravel](https://laravel.com/)

The project is based on [ES2015+](http://es6.ruanyifeng.com/), [vue](https://cn.vuejs.org/index.html), [vuex](https://vuex.vuejs.org/zh-cn/), [vue-router](https://router.vuejs.org/zh-cn/), [axios](https://github.com/axios/axios) and [element-ui](https://github.com/ElemeFE/element).

## API
API will be served by Laravel. In this project, you need to run migration and data feeder to generate sample data for authentication/authorization, other APIs will be faked.

## Getting started
You have to check installation guide of Laravel (https://laravel.com/docs/5.7)

```bash
# Clone the project and run composer
git clone https://github.com/SeniorDev34/Laravel-Vue-Dashboard.git
cd Laravel-Vue-Dashboard
composer install

# Create .env from .env.example
cp .env.example .env

# Generate application key
php artisan key:generate

# Migration and DB seeder (after changing your DB settings in .env)
php artisan migrate --seed

# Generate JWT secret key
php artisan jwt:secret

# install dependency
npm install

# develop
npm run dev
```

## Deployment and/or CI/CD
This project uses [Envoy](https://laravel.com/docs/5.7/envoy) for deployment, and [GitLab CI/CD](https://about.gitlab.com/product/continuous-integration/). Please check `Envoy.blade.php` and `.gitlab-ci.yml` for more detail.
