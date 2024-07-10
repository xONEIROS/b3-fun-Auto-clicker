# b3-fun--Auto-clicker

<div align="center">
![UntitledProject0000-ezgif com-video-to-gif-converter-min](https://github.com/xONEIROS/b3-fun--Auto-clicker/assets/174752031/8021f9d6-5a0c-4879-b866-a474df00719b)
</div>
## برای به دست آوردن پوینت های b3.fun کد زیر را در داخل قسمت کنسول مرورگر پیست کنید و روی وسط صفحه یک بار کلیک کنید تا کلیکر بصورت اتوماتیک بجای شما کلیم کند
**در کد زیر میتونید مقادیر زیر را تغییر دهید**
مقادیر `const m = 5000, t = 100, r = 19;` به ترتیب `m` برای تعداد کلیک هایی که نیاز دارد در اینجا پس از 5000 بار کیک کد متوقف میشود ، مقدار `t` فاصله بین هر کلیک بر اساس میلی ثانیه ( بهتره این مقدار رو زیر 100 میلی ثانیه قرار ندید ) چون ثبت نمیشن امتیاز ها .

```
document.addEventListener('click', function(e) {
    alert('لطفا به کانال تلگرام ما بپیوندید https://t.me/xOneiros');
    let c = 0;
    const m = 5000, t = 100, r = 19;
    function rp(a, b) {
        const ang = Math.random() * 2 * Math.PI;
        const x = a.x + b * Math.cos(ang);
        const y = a.y + b * Math.sin(ang);
        return { x, y };
    }
    function k() {
        if (c >= m) {
            clearTimeout(i);
            return;
        }
        const { x, y } = rp({ x: e.clientX, y: e.clientY }, r);
        const a = new MouseEvent('click', { view: window, bubbles: true, cancelable: true, clientX: x, clientY: y });
        document.elementFromPoint(x, y).dispatchEvent(a);
        c++;
        i = setTimeout(k, t);
    }
    let i = setTimeout(k, t);
    document.removeEventListener('click', arguments.callee);
});
```


<div align="center">
    <p>
        <a href="Https://x.com/0xOneiros">
            <small>twitter</small>  
        </a>
        | 
        <a href="Https://t.me/xOneiros">
            <small>telegram</small>  
        </a>
    </p>
</div>
