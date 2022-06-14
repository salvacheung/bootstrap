---
layout: docs
title: 徽章
description: 文档与案例
group: components
toc: true
---

## 案例

徽章通过使用相对字体大小和 `em` 单位来缩放以匹配直接父元素的大小。从 v5 开始，徽章不再具有链接的焦点或悬停样式。

### 标题

{{< example >}}
<h1>Example 威威 heading <span class="badge bg-secondary">New</span></h1>
<h2>Example heading <span class="badge bg-secondary">New</span></h2>
<h3>Example heading <span class="badge bg-secondary">New</span></h3>
<h4>Example heading <span class="badge bg-secondary">New</span></h4>
<h5>Example heading <span class="badge bg-secondary">New</span></h5>
<h6>Example heading <span class="badge bg-secondary">New</span></h6>
{{< /example >}}

### 按钮

{{< example >}}
<button type="button" class="btn btn-primary">
  Notifications <span class="badge text-bg-secondary">4</span>
</button>
{{< /example >}}

### 定位

{{< example >}}
<button type="button" class="btn btn-primary position-relative">
  Inbox
  <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-danger">
    99+
    <span class="visually-hidden">unread messages</span>
  </span>
</button>
{{< /example >}}


{{< example >}}
<button type="button" class="btn btn-primary position-relative">
  Profile
  <span class="position-absolute top-0 start-100 translate-middle p-2 bg-danger border border-light rounded-circle">
    <span class="visually-hidden">New alerts</span>
  </span>
</button>
{{< /example >}}

## 背景颜色

{{< added-in "5.2.0" >}}


{{< example >}}
{{< badge.inline >}}
{{- range (index $.Site.Data "theme-colors") }}
<span class="badge text-bg-{{ .name }}">{{ .name | title }}</span>{{- end -}}
{{< /badge.inline >}}
{{< /example >}}

## 药丸徽章

{{< example >}}
{{< badge.inline >}}
{{- range (index $.Site.Data "theme-colors") }}
<span class="badge rounded-pill text-bg-{{ .name }}">{{ .name | title }}</span>{{- end -}}
{{< /badge.inline >}}
{{< /example >}}

## 徽章组

{{< example >}}
{{< badge.inline >}}
{{- range (index $.Site.Data "theme-colors") }}
<span class="badge">{{ .name | title }}</span>
<span class="badge-group">
  <span class="badge text-bg-{{ .name }}">{{ .name | title }}</span>
  <span class="badge text-bg-red-200">徽章</span>
</span>{{- end -}}
{{< /badge.inline >}}
{{< /example >}}

## CSS

### Variables

{{< added-in "5.2.0" >}}

As part of Bootstrap's evolving CSS variables approach, badges now use local CSS variables on `.badge` for enhanced real-time customization. Values for the CSS variables are set via Sass, so Sass customization is still supported, too.

{{< scss-docs name="badge-css-vars" file="scss/_badge.scss" >}}

### Sass variables

{{< scss-docs name="badge-variables" file="scss/_variables.scss" >}}
