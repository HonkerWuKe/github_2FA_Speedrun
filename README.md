# GitHub 2FA 验证码生成器

一个简单易用的浏览器扩展，帮助用户生成 GitHub 双重认证（2FA）的验证码。

## 主要功能

- 生成 GitHub 双重认证的 6 位验证码
- 30 秒自动更新验证码
- 支持导入和管理恢复码
- 简洁的用户界面
- 安全的本地密钥存储

## 使用方法

1. 在 GitHub 设置 2FA 时，复制 "Your two-factor secret" 密钥
2. 将密钥输入插件，点击"开始生成"
3. 查看实时更新的验证码
4. 可选：导入恢复码以便统一管理

## 安全说明

- 所有数据均在本地存储，不会上传到任何服务器
- 密钥使用浏览器安全存储机制保护
- 建议妥善保管恢复码

## 技术实现

- 使用 Web Crypto API 进行 TOTP 计算
- 基于 Chrome Extension Manifest V3
- 支持 Firefox 浏览器（需要 v109.0 或更高版本）

## 开发相关

- 使用 JavaScript/HTML/CSS 开发
- 实现了标准的 TOTP 算法
- 支持 Base32 密钥解码

## 许可证

MIT License 