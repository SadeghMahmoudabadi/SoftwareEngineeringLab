# SoftwareEngineeringLab
## پرسش‌ها
### پرسش ۱
پوشه .git مرکز یک repository گیت‌هاب است. این پوشه برای نگهداری اطلاعات مدیریت نسخ پروژه استفاده می‌شود؛ شامل تاریخچه commitها، اطلاعات شاخه‌ها، حزئیات repository، تغییرات فایل‌ها و ....
این پوشه با دستور git init ساخته می‌شود.
### پرسش ۲
اصطلاح atomic وقتی به کار می‌رود که تمرکز روی یک بهش مجزای پروژه باشد، نه چندین بخش نامرتبط.

ویژگی‌های atomic commit به شرح زیر هستند:
* یک تغییر منطقی است، نه چندین تغییر نامرتبط.
* کامل است. به این معنی که کاربردی به کد اضافه می‌کند و یک قدم رو به جلو محسوب می‌شود.
* ایزوله است و به تغییراتی که هنوز commit نشده‌اند وابسته نیست.

ویژگی‌های atomic pull request به شرح زیر هستند:
  * مربوط به یک مسئله، باگ، یا feature خاص است.
  * تغییرات پس از pull request باید در چند سری atomic commit اعمال شوند.
  * باید به صورت کامل بررسی شود، حتی اگر از چند commit مختلف تشکیل شده باشد.
### پرسش ۳
* ‎‌‌‌fetch: تغییرات اعمال شده در remote repository را دانلود می‌کند،، ولی شاخه فعلی را تغییر نمی‌دهد.
* ‎pull: تغییرات اعمال شده در remote repository را دانلود می‌کند و در شاخه فعلی نیز اعمال می‌کند.
* ‎merge: یک commit جدید درست می‌کند و تغییرات شاخه فعلی و شاخه دیگری که درخواست merge به آن زده شده است را ترکیب می‌کند.
* ‎rebase: تاریخچه شاخه فعلی را بازنویسی می‌کند، به گونه ای که commitهای این شاخه را به صورت خطی به نسخه شاخه دیگری جایگذاری می‌کند به طوری که انگار از اول به همین ترتیب بوده است.
* ‎cherry-pick: به ما حق انتخاب از بین commitهای یک شاخه دیگر برای merge می‌دهد. به این ترتیب، می‌توانیم فقط یک سری آیتم دلخواه از شاخه دیگر دریافت کنیم.
### پرسش ۴
* reset: تاریخچه پروژه را تغییر می‌دهد و اشاره‌گر HEAD که به آخرین commit اشاره می‌کند را جا به جا می‌کند.
* revert: یک commit جدید درست می‌کند و تغییرات اعمال شده در commit دیگری را بازگردانی می‌کند. تفاوت آن با reset این است که تاریخچه پروژه را تغییر نمی‌دهد.
* restore: برای بازگردانی یک فایل خاص یا فهرست کاری استفاده می‌شود که معمولا به صورت تصادفی پاک یا عوض شده اند.
* switch: شاخه را به آخرین شاخه که اشاره‌گر HEAD اشاره می‌کند تغییر می‌دهد و فایل‌ها را بروزرسانی می‌کند.
* checkout: عملکردی مشابه switch دارد، با این تفاوت که به شاخه دلخواه تغییر می‌کند.
