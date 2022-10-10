# THEME - RIPPLE 2022 - OPHIM CMS

## Demo

## Requirements
https://github.com/hacoidev/ophim-core

## Install
1. Tại thư mục của Project: `composer require hacoidev/ophim-ripple`
2. Kích hoạt giao diện trong Admin Panel

## Update
1. Tại thư mục của Project: `composer update hacoidev/ophim-ripple`

## Document
### List
- Trang chủ: `display_label|relation|find_by_field|value|limit|show_more_url`
    + Ví dụ theo định dạng: `Phim bộ mới||type|series|12|/danh-sach/phim-bo`
    + Ví dụ theo định dạng: `Phim lẻ mới||type|single|12|/danh-sach/phim-le`
    + Ví dụ theo thể loại: `Phim hành động|categories|slug|hanh-dong|12|/the-loai/hanh-dong`
    + Ví dụ theo quốc gia: `Phim hàn quốc|regions|slug|han-quoc|12|/quoc-gia/han-quoc`
    + Ví dụ với các field khác: `Phim chiếu rạp||is_shown_in_theater|1|12|/danh-sach/phim-chieu-rap|`

- Danh sách hot: `Label|relation|find_by_field|value|sort_by_field|sort_algo|limit`
    + `Phim sắp chiếu||status|trailer|publish_year|desc|9`
    + `Top phim bộ||type|series|view_total|desc|9`
    + `Top phim lẻ||type|single|view_total|desc|9`

### Custom View Blade
- File blade gốc trong Package: `/vendor/hacoidev/ophim-ripple/resources/views/ripple`
- Copy file cần custom đến: `/resources/views/vendor/themes/ripple`
