# SoftwareEngineeringLab
## گزارش کار
در این آزمایش، یک صفحه HTML static برای نمایش رزومه طراحی شده است. ابتدا شاخه main در تنظیمات protected شده است تا فقط با pull request بتوان به آن دسترسی پیدا کرد. در شاخه dev، پیاده‌سازی صفحات وب انجام شده است. پس از بررسی نسخه اولیه dev، با مشکل اشتباه اسمی یکی از تب‌ها مواجه شدیم که در شاخه debug آن را رفع کردیم. در شاخه feature، اطلاعات تماس به عنوان feature رزومه اضافه شده است. اما به دلیل همزمانی تغییرات در شاخه debug، به دو conflict برخوردیم که هنگام pull request آنها را برطرف کردیم. تلاش شد از تمامی دستورات ذکرشده در 
![Screenshot 2024-03-08 113722](https://github.com/SadeghMahmoudabadi/SoftwareEngineeringLab/assets/59364741/ab2d0fc8-d166-43d1-a200-eefbb3420330)
<img width="682" alt="Screenshot 2024-03-08 at 7 14 50 PM" src="https://github.com/SadeghMahmoudabadi/SoftwareEngineeringLab/assets/59364741/497199f2-baed-48d9-b819-d7249557ac86">
<img width="682" alt="Screenshot 2024-03-08 at 7 17 39 PM" src="https://github.com/SadeghMahmoudabadi/SoftwareEngineeringLab/assets/59364741/4e72d91b-77c6-49d3-893a-67d39e68cd52">
<img width="682" alt="Screenshot 2024-03-08 at 7 19 39 PM" src="https://github.com/SadeghMahmoudabadi/SoftwareEngineeringLab/assets/59364741/5db63ee0-0689-4b4a-8a6b-0deb4dca4fa4">
![photo_2024-03-08_20-27-53](https://github.com/SadeghMahmoudabadi/SoftwareEngineeringLab/assets/59364741/682c7ff3-8e74-4746-8fe4-2e206eb2ae4d)
![photo_2024-03-08_20-27-43](https://github.com/SadeghMahmoudabadi/SoftwareEngineeringLab/assets/59364741/6cd774a1-793f-49e5-a74a-d429a090a5ac)
<img width="682" alt="Screenshot 2024-03-08 at 7 21 55 PM" src="https://github.com/SadeghMahmoudabadi/SoftwareEngineeringLab/assets/59364741/ecc6059c-e95c-4cd1-85b6-ca90fea1a2b5">
![Screenshot 2024-03-08 193055](https://github.com/SadeghMahmoudabadi/SoftwareEngineeringLab/assets/59364741/34da5f80-3e15-48d3-b6eb-4c0cbc2acc87)
![Screenshot 2024-03-08 193119](https://github.com/SadeghMahmoudabadi/SoftwareEngineeringLab/assets/59364741/8edee8f8-aca9-4a09-a6c3-e8721438e642)
![Screenshot 2024-03-08 193315](https://github.com/SadeghMahmoudabadi/SoftwareEngineeringLab/assets/59364741/fc88d1a6-31af-49af-9506-4a7fe3c7a950)
<img width="822" alt="Screenshot 2024-03-08 at 7 50 01 PM" src="https://github.com/SadeghMahmoudabadi/SoftwareEngineeringLab/assets/59364741/0f0eee00-2a2a-428b-bae9-907493a5eaf1">
<img width="682" alt="Screenshot 2024-03-08 at 12 19 04 PM" src="https://github.com/SadeghMahmoudabadi/SoftwareEngineeringLab/assets/59364741/783db1fc-c29f-45c6-bf97-815373f86c21">
<img width="682" alt="Screenshot 2024-03-08 at 12 19 40 PM" src="https://github.com/SadeghMahmoudabadi/SoftwareEngineeringLab/assets/59364741/31697f07-7403-483b-9dee-327676734019">
<img width="934" alt="Screenshot 2024-03-08 at 12 21 21 PM" src="https://github.com/SadeghMahmoudabadi/SoftwareEngineeringLab/assets/59364741/c1fe0149-6d2c-4cd9-95f9-bc5a0fb99bac">



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
* ا fetch: تغییرات اعمال شده در remote repository را دانلود می‌کند،، ولی شاخه فعلی را تغییر نمی‌دهد.
* ا pull: تغییرات اعمال شده در remote repository را دانلود می‌کند و در شاخه فعلی نیز اعمال می‌کند.
* ا merge: یک commit جدید درست می‌کند و تغییرات شاخه فعلی و شاخه دیگری که درخواست merge به آن زده شده است را ترکیب می‌کند.
* ا rebase: تاریخچه شاخه فعلی را بازنویسی می‌کند، به گونه ای که commitهای این شاخه را به صورت خطی به نسخه شاخه دیگری جایگذاری می‌کند به طوری که انگار از اول به همین ترتیب بوده است.
* ا cherry-pick: به ما حق انتخاب از بین commitهای یک شاخه دیگر برای merge می‌دهد. به این ترتیب، می‌توانیم فقط یک سری آیتم دلخواه از شاخه دیگر دریافت کنیم.
### پرسش ۴
* ا reset: تاریخچه پروژه را تغییر می‌دهد و اشاره‌گر HEAD که به آخرین commit اشاره می‌کند را جا به جا می‌کند.
* ا revert: یک commit جدید درست می‌کند و تغییرات اعمال شده در commit دیگری را بازگردانی می‌کند. تفاوت آن با reset این است که تاریخچه پروژه را تغییر نمی‌دهد.
* ا restore: برای بازگردانی یک فایل خاص یا فهرست کاری استفاده می‌شود که معمولا به صورت تصادفی پاک یا عوض شده اند.
* ا switch: شاخه را به آخرین شاخه که اشاره‌گر HEAD اشاره می‌کند تغییر می‌دهد و فایل‌ها را بروزرسانی می‌کند.
* ا checkout: عملکردی مشابه switch دارد، با این تفاوت که به شاخه دلخواه تغییر می‌کند.
### پرسش ۵
در گیت، stage یا index یک محل نگهداری موقت برای تغییراتی است که برای commit بعدی برنامه‌ریزی شده‌اتد. این عمل با دستور 'git add 'file name انجام می‌شود.
### پرسش ۶
در گیت، snapshot یک حالت ذخیره شده از پروژه در یک زمان مشخص است. snapshot شامل تمامی فایل‌های پروژه به صورت فشرده است که برای بازگردانی پروژه به نسخه مدنظر استفاده می‌شود.

با هر commit، یک snapshot از پروژه ایجاد می‌شود که مربوط به ورژن commit شده است. در کلامی دیگر، commit روند ایجاد یک snapshot با توضیحاتی در مورد تغییرات اعمال شده است.

دستور stash برای بازگردانی و ذخیره تغییرات commit نشده یا stage شده است. با اجرای این دستور، به آخرین نسخه پروژه که pull کرده‌ایم بازمی‌گردیم. می‌توان از حالت stash شده، تغییراتی که اعمال کرده بودیم را برگردانیم.
### پرسش ۷
ویژگی‌های local repository: در سیستم فردی قرار دارد. به صورت انفرادی می‌شود روی آن کار کرد. نیاز به اینترنت ندارد. می‌توان با اطمینان خاطر روی آن آزمون و خطا کرد بدون اینکه به پروژه آسیبی وارد شود. به صورت پیش‌فرض فقط توسط صاحب سیستم قابلیت دسترسی دارد.

ویژگی‌های remote repository: در سرور راه دور قرار دارد، مانند Github. برای همکاری تیمی و مدیریت نسخه‌های پروژه استفاده می‌شود. نیاز به اینترنت دارد. ممکن است به پروژه آسیب بزند و بهتر است برای آزمون و خطا استفاده نشود. برای دسترسی نیاز به اجازه مدیر پروژه در سرور دارد.
