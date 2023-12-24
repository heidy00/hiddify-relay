# all-in-one
all tunnel in one bash


.با این اسکریپت شما میتونید 4 روش تانل زدن بین سرور ایران و خارج انجام بدید

1.`IP Tables`

2.`GOST`

3.`Xray-dokodemo`

4.`HAProxy`


![image](https://github.com/HiddifySupport-Return/hiddify-relay/assets/151555003/23e2073a-881d-4d37-bfe0-cf43a85b2098)


## دستور اجرای اسکریپت

```
bash -c "$(curl -L https://raw.githubusercontent.com/hiddify/hiddify-relay/main/install.sh)"
```

## آموزش استفاده از اسکریپت

 - به  سرور میانی [SSH بزنید](https://github.com/hiddify/Hiddify-Manager/wiki/SSH-%D8%A2%D9%85%D9%88%D8%B2%D8%B4-%D8%A7%D8%AA%D8%B5%D8%A7%D9%84-%D8%A8%D9%87-%D8%B3%D8%B1%D9%88%D8%B1-%D8%A7%D8%B2-%D8%B7%D8%B1%DB%8C%D9%82) و دستور اسکریپت را اجرا کنید.

## تانل IPTables


مطابق تصویر بالا شماره `1` را انتخاب نماید و وارد منوی تانل `IPTables` شوید:

1.نصب و راه اندازی تانل
- پس از انتخاب شماره یک در تانل `IPTables` از شما آدرس `IP` سرور اصلی را میخواهد وارد نماید و دکمه `Enter` را فشارد دهید تا تانل بروی پورت `443` و `80` فعال سازی شود.

2.نمایش پورت های مورد استفاده شده دز تانل `IPTables`

3.پاکسازی تانل `IPTables` و قواعد تانل
- دقت داشته باشد که اگر قواعد خاصی در کنار تانل به صورت دستی ایجاد کرده باشید با این دستور پاک خواهند شد.

4.خروج از منو تانل `IPTables`

## تانل GOST

برای استفاده تانل `GOST` شماره `2` را در منوی اصلی انتخاب نمایید:

1.نصب تانل `GOST` 
- پس از انتخاب شماره `1` منتظر بمانید تا تانل نصب شود پس از اتمام نصب در مرحله اول باید `Port` مورد نظر را برای تانل وارد نماید و سپس `Enter` بزنید در مرحله بعد دامنه یا ساب دامنه سرور اصلی خود را وارد نماید سپس `Enter` بزنید منتظر بمانید تا تانل راه اندازی شود پس از راه اندازی پیام `Gost install and enabled` به رنگ سبز نمایش داده میشود.

2.چک کردن `Port` و `Active` بودن تانل `GOST`
- پس از انتخاب گزینه `2` پورت مورد استفاده شده در تانل و فعال بودن تانل به شما نمایش داده میشود.

3.افزودن پورت و دامنه دیگر
- درصورتی که میخواهد از سرور میانی به چند سرور خارج خود تانل بزیند میتوانید از این گزینه استفاده نمایید.
- پس از انتخاب عدد `3` باید `Port` جدید را وارد نماید دکمه `Enter` را بزنید سپس دامنه سرور خارج را وارد نماید و دکمه `Enter` را بزنید پس از انجام عملیات پیام `New port and domain added` دریافت خواهید کرد که به منزله انجام درست عملیات میباشد.
- میتوانید برای اطمینان از درست بودن مراحل گزینه شماره `2` را وارد نماید و پورت های مورد استفاده و فعال بودن تانل را چک نمایید.

4. حذف تانل `GOST` از سرور میانی شما

5.خروج از منوی تانل `GOST`

## تانل XRAY (Dokodemo-door)

برای استفاده از تانل `Dokodemo-door` شماره `3` را وارد نماید.

1.نصب و راه اندازی تانل
- پس از انتخاب شماره `1` در منوی تانل `Dokodemo-door` منتظر بمانید تا هسته `Xray` برای شما نصب شود.
- پس از نصب در قسمت `Enter the address` آدرس `IP` سرور اصلی یا دامنه سرور اصلی خورد را وارد نماید سپس در قسمت `Enter the port` پورت موردنظر تانل را وارد نمایید (پیشنهادی : `443`,`80`) سپس دکمه `Enter` بزنید با نمایش پیغام `Inbound added and tunnel started` تانل شما راه اندازی میشود.

2.چک کردن `Port` و `Active` بودن تانل `Dokodemo-door`
- پس از انتخاب گزینه `2` پورت مورد استفاده شده در تانل و فعال بودن تانل به شما نمایش داده میشود.

3.افزدون اینباند
- میتواند با گزینه `3` در منوی تانل `Dokodemo-door` اینباند دیگری ایچاد نمیاد و سرور میانی خود را به چند سرور خارج متصل نمایید
- پس از انتخاب گزینه `3` در قسمت `Enter the new address` دامنه سرور یا `IP` سرور جدید خارج خود را وارد نمایید سپس `Enter` نمایید ، مرحله بعد در قسمت `Enter the new port` پورت جدید وارد نمایید و دکمه `Enter` را بزنید پس از انجام درست عملیات پیغام `Additional inbound added` خواهید دید.
- میتوانید برای اطمینان از درست بودن مراحل گزینه شماره `2` را وارد نماید و پورت های مورد استفاده و فعال بودن تانل را چک نماید.

4.حذف تانل `Dokodemo-door` و هسته ی `Xray` از سرور میانی شما

5.خروج از منوی تانل `Dokodemo-door`

## تانل HAProxy

برای استفاده از تانل `HAProxy` شماره `4` انتخاب نمایید.

1.نصب و راه اندازی تانل
- پس از انتخاب گزینه `1` منتظر نصب بسته `HAProxy` بمانید 
- سپس بعد از نصب در قسمت `Enter Iran-Server Free Port` پورت مورد نظر در سرور ایران را وارد نمایید(پیشنهادی پورت 443)
- سپس در قسمت `Enter Main-Server IP` آدرس IP سرور اصلی و خارج خود را وارد نمایید.
- سپس در قسمت `Enter Main-Server Port` پورت آزاد شده در سرور اصلی و خارج خود را وارد نمایید(به طور پیشفرض هیدیفای از پورت 443 استفاده میکند که پیشنهاد میشود از همین پورت استفاده نمایید).
- بعد از انجام درست عملیات پیغام `HAProxy installed and active successfully!` برای شما نمایش داده خواهد.

2.چک کردن پورت های مورد استفاده تانل `HAProxy` و فعال بودن سرویس تانل `HAProxy`

3.حذف تانل `HAProxy` از سرور میانی

4.خروج از منوی تانل `HAProxy`

## تعریف سرور میانی در هیدیفای
حالا برای آیپی سرور میانی (ایران) خود یک ساب‌دامین با پروکسی خاموش ثبت نمایید و آن را در هیدیفای روی حالت Relay ثبت نمایید.

<img src="https://user-images.githubusercontent.com/125398461/235341283-97c026b7-1d70-4362-8950-1e5c1b79d508.png">

## افزودن کانفیگ‌های Relay جهت استفاده به لینک سابسکریپشن

همانند همیشه در هیدیفای بهتر است کانفیگ‌ها را از لینک سابسکریپشن جدا کنید. بنابراین برای دامنه Relay ثبت شده نیز می‌توانید در تنظیمات دامنه مربوط به سابسکریپشن، تیک مربوط به دامین Relay را بزنید تا کانفیگ‌های آن به دامنه سابسکریپشن اضافه گردند.

فرض شود که دامنه مربوط به سابسکریپشن t1.hiddify.com باشد، مطابق با تصویر زیر جلو بروید تا کار انجام شود.
<img src="https://user-images.githubusercontent.com/125398461/235342038-cfda2574-2444-4414-843d-2ed507537d1d.png">

حالا اگه صفحه کاربر را با دامین سابسکریپشن (در اینجا t1.hiddify.com) باز نمایید خواهید دید که کانکشن‌های مربوط به Relay نیز اضافه شده‌اند. می‌توانید این کانکشن‌ها را به صورت تک تک و یا با استفاده از لینک‌های سابسکریشن معمولی یا سابسکریپشن b64 به کلاینت خود اضافه نمایید و استفاده نمایید.


