<p align="center">
    <img src="doc/demo/logo.png" width="80px" />
    <h1 align="center">Cloud Mail</h1>
    <p align="center">A simple, responsive email service built on Cloudflare, with email sending and attachment support 🎉</p> 
    <p align="center">
        Main README (English) | <a href="/README-en.md" style="margin-left: 5px">English </a>
    </p>
    <p align="center">
        <a href="https://github.com/maillab/cloud-mail/tree/main?tab=MIT-1-ov-file" target="_blank" >
            <img src="https://img.shields.io/badge/license-MIT-green" />
        </a>    
        <a href="https://github.com/maillab/cloud-mail/releases" target="_blank" >
            <img src="https://img.shields.io/github/v/release/maillab/cloud-mail" alt="releases" />
        </a>  
        <a href="https://github.com/maillab/cloud-mail/issues" >
            <img src="https://img.shields.io/github/issues/maillab/cloud-mail" alt="issues" />
        </a>  
        <a href="https://github.com/maillab/cloud-mail/stargazers" target="_blank">
            <img src="https://img.shields.io/github/stars/maillab/cloud-mail" alt="stargazers" />
        </a>  
        <a href="https://github.com/maillab/cloud-mail/forks" target="_blank" >
            <img src="https://img.shields.io/github/forks/maillab/cloud-mail" alt="forks" />
        </a>
    </p>
    <p align="center">
        <a href="https://trendshift.io/repositories/20459" target="_blank" >
            <img src="https://trendshift.io/api/badge/repositories/20459" alt="trendshift" >
        </a>
    </p>
</p>


## Project Overview

With just one domain, you can create multiple email addresses, similar to major email platforms. Deploy this project to Cloudflare Workers to reduce server costs and run your own email service.

## Project Showcase

- [Live Demo](https://skymail.ink)<br>
- [Deployment Guide](https://doc.skymail.ink)<br>

| ![](/doc/demo/demo1.png) | ![](/doc/demo/demo2.png) |
|-----------------------|-----------------------|
| ![](/doc/demo/demo3.png) | ![](/doc/demo/demo4.png) |




## Features

- **💰 Low-Cost Hosting**: Deploy to Cloudflare Workers to reduce server costs

- **💻 Responsive Design**: The layout automatically adapts to desktop and most mobile browsers

- **📧 Email Sending**: Send email through Resend, with bulk sending, inline images, attachments, and delivery-status tracking

- **🛡️ Administration**: Manage users and email, with role-based access control for features and resource limits

- **📦 Attachments**: Send and receive attachments, using R2 object storage to save and download files

- **🔔 Email Forwarding**: Forward received messages to Telegram bots or mailboxes hosted by other providers

- **📡 Open API**: Create users in bulk and query email with multiple filters through the API 

- **🔢 Verification Code Recognition**: Automatically detect email verification codes with Workers AI 

- **📈 Data Visualization**: Visualize system data and user/email growth with ECharts

- **🎨 Personalization**: Customize the site title, login background, and transparency

- **🤖 CAPTCHA**: Use Turnstile verification to prevent automated bulk registration

- **📜 More Features**: Under development...



## Tech Stack

- **Platform**：[Cloudflare Workers](https://developers.cloudflare.com/workers/)

- **Web Framework**：[Hono](https://hono.dev/)

- **ORM：**[Drizzle](https://orm.drizzle.team/)

- **Frontend Framework**：[Vue3](https://vuejs.org/) 

- **UI Framework**：[Element Plus](https://element-plus.org/) 

- **Email Service：** [Resend](https://resend.com/)

- **Cache**：[Cloudflare KV](https://developers.cloudflare.com/kv/)

- **Database**：[Cloudflare D1](https://developers.cloudflare.com/d1/)

- **File Storage**：[Cloudflare R2](https://developers.cloudflare.com/r2/)

## Project Structure

```
cloud-mail
├── mail-worker				    # Backend worker project
│   ├── src                  
│   │   ├── api	 			    # API layer			
│   │   ├── const  			    # Project constants
│   │   ├── dao                 # Data access layer
│   │   ├── email			    # Email processing and receiving
│   │   ├── entity			    # Database entities
│   │   ├── error			    # Custom exceptions
│   │   ├── hono			    # Web framework configuration, middleware, and global error handling
│   │   ├── i18n			    # Internationalization
│   │   ├── init			    # Database and cache initialization
│   │   ├── model			    # Response data models
│   │   ├── security			# Authentication and authorization
│   │   ├── service			    # Business logic layer
│   │   ├── template			# Message templates
│   │   ├── utils			    # Utility functions
│   │   └── index.js			# Entry point
│   ├── pageckge.json			# Project dependencies
│   └── wrangler.toml			# Project configuration
│
├── mail-vue				    # Frontend Vue project
│   ├── src
│   │   ├── axios 			    # Axios configuration
│   │   ├── components			# Custom components
│   │   ├── echarts			    # ECharts integration
│   │   ├── i18n			    # Internationalization
│   │   ├── init			    # Startup initialization
│   │   ├── layout			    # Main layout components
│   │   ├── perm			    # Access control
│   │   ├── request			    # API requests
│   │   ├── router			    # Router configuration
│   │   ├── store			    # Global state management
│   │   ├── utils			    # Utility functions
│   │   ├── views			    # Page components
│   │   ├── app.vue			    # Root component
│   │   ├── main.js			    # Entry JavaScript file
│   │   └── style.css			# Global CSS
│   ├── package.json			# Project dependencies
└── └── env.release				# Project configuration
```

## Sponsor

<a href="https://doc.skymail.ink/support.html" >
<img width="170px" src="./doc/images/support.png" alt="">
</a>

## License

This project is licensed under the [MIT](LICENSE) license.	


## Community

[Telegram](https://t.me/cloud_mail_tg)



