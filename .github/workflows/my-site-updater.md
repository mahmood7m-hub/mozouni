---
engine:
  id: copilot
  model: gpt-4o
on:
  schedule:
    - cron: '0 0 * * 0'
  workflow_dispatch:
on:
  schedule:
    - cron: '0 0 * * 0'
  workflow_dispatch:

permissions:
  contents: read

safe-outputs:
  create-pull-request:
    max: 1
---

# به‌روزرسانی محتوای سایت

فایل index.html را بخوان و محتوای آن را بررسی کن.

اگر بخش "اخبار" یا "مقالات" یا "محصولات" در آن وجود دارد، آنها را با اطلاعات جدید و به‌روز به‌روزرسانی کن.

تغییرات را در قالب یک Pull Request پیشنهاد بده و در توضیحات PR بنویس که چه چیزی تغییر کرده است.

فقط فایل index.html را تغییر بده.
