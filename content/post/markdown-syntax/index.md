+++
author = "Ula"
title = "Hướng dẫn cú pháp Markdown."
date = "2019-03-11"
description = "Bài viết mẫu giới thiệu cú pháp Markdown cơ bản và định dạng cho các phần tử HTML."
tags = [
    "markdown",
    "css",
    "html",
    "themes",
]
categories = [
    "themes",
    "syntax",
]
series = ["Themes Guide"]
aliases = ["migrate-from-jekyl"]
image = "pawel-czerwinski-8uZPynIu-rQ-unsplash.jpg"
+++

Bài viết này cung cấp một mẫu cú pháp Markdown cơ bản được sử dụng trong file nội dung của Hugo, nó cũng cho thấy liêu các yếu tô HTML cơ bản có được trang trí với css trong theme Hugo hay không.

<!--more-->

## Headings

Các phần tử của HTML `<h1>`—`<h6>` thể hiện cho 6 cấp độ của các phần `<h1>` là mức độ cao nhất trong khi `<h6>` là cấp độ thấp nhất.

# H1
## H2
### H3
#### H4
##### H5
###### H6

## Paragraph

Mạng 4G là tên viết tắt của Fourth-Generation, đây là công nghệ truyền thông không dây cho phép truyền tải dữ liệu tối đa lên tới 1 - 1.5Gb/giây ở điều kiện lý tưởng. Các tiêu chuẩn thiết lập cho kết nối 4G được Tổ chức kết nối mạng thế giới ITU-R ban hành vào tháng 3 năm 2008, đòi hỏi tất cả các dịch vụ có 4G phải tuân thủ đúng một loạt các tiêu chuẩn về đường truyền tốc độ và kết nối.

Mạng LTE là thuật ngữ có tên tiếng Anh là Long Term Evolution, được hiểu nôm na là “Tiến hóa dài hạn”. Mạng LTE không được xem là một công nghệ mạng, thay vào đó LTE chỉ là một tiêu chuẩn công nghệ được cải tiến từ các chuẩn GSM.UMTS.

## Blockquotes

Phần tử blockquote đại diện cho nội dung được trích dẫn từ một nguồn khác, tùy chọn với phần trích dẫn phải nằm trong phần tử `footer` hoặc `cite`, và tùy chọn với các thay đổi trong dòng như chú thích và chữ viết tắt.


#### Blockquote mà không attribution

> Tiam, ad mint andaepu dandae nostion secatur sequo quae.
> **Note** that you can use *Markdown syntax* within a blockquote.

#### Blockquote với attribution

> Don't communicate by sharing memory, share memory by communicating.<br>
> — <cite>Rob Pike[^1]</cite>

[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

## Tables

Các bảng không phải là một phần của Markdown cốt lõi, nhưng Hugo hỗ trợ hỗ trợ chúng.

   Name | Age
--------|------
    Bob | 27
  Alice | 23

#### Inline Markdown within tables

| Italics   | Bold     | Code   |
| --------  | -------- | ------ |
| *italics* | **bold** | `code` |

| A                                                        | B                                                                                                             | C                                                                                                                                    | D                                                 | E                                                          | F                                                                    |
|----------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------|------------------------------------------------------------|----------------------------------------------------------------------|
| Lorem ipsum dolor sit amet, consectetur adipiscing elit. | Phasellus ultricies, sapien non euismod aliquam, dui ligula tincidunt odio, at accumsan nulla sapien eget ex. | Proin eleifend dictum ipsum, non euismod ipsum pulvinar et. Vivamus sollicitudin, quam in pulvinar aliquam, metus elit pretium purus | Proin sit amet velit nec enim imperdiet vehicula. | Ut bibendum vestibulum quam, eu egestas turpis gravida nec | Sed scelerisque nec turpis vel viverra. Vivamus vitae pretium sapien |

## Code Blocks

#### Code block with backticks

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```

#### Code block indented with four spaces

    <!doctype html>
    <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>Example HTML5 Document</title>
    </head>
    <body>
      <p>Test</p>
    </body>
    </html>

#### Code block with Hugo's internal highlight shortcode
{{< highlight html >}}
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

#### Diff code block

```diff
[dependencies.bevy]
git = "https://github.com/bevyengine/bevy"
rev = "11f52b8c72fc3a568e8bb4a4cd1f3eb025ac2e13"
- features = ["dynamic"]
+ features = ["jpeg", "dynamic"]
```

## List Types

#### Ordered List

1. First item
2. Second item
3. Third item

#### Unordered List

* List item
* Another item
* And another item

#### Nested list

* Fruit
  * Apple
  * Orange
  * Banana
* Dairy
  * Milk
  * Cheese

## Other Elements — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.

## Hyperlinked image

[![Google](https://www.google.com/images/branding/googlelogo/1x/googlelogo_light_color_272x92dp.png)](https://google.com)