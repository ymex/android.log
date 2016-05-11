# cute.L
Log printer for Android

##Use in Android Studio

```
dependencies {
    compile 'cn.ymex:cute.L:0.5.2'
}
```

##Sample Usage


```java
 @Override
    public void onClick(View v) {
        switch (v.getId()) {
            case R.id.btn_base://base type
                L.i(1);
                L.d(2.0);
                L.e(false);
                L.w("this is String type!");
                break;
            case R.id.btn_ob://object type
                L.d(Data.object());
                break;
            case R.id.btn_null:// object is null
                L.d(null);
                break;
            case R.id.btn_list: // list type
                L.d(Data.list());
                break;
            case R.id.btn_map://map type
                L.w(Data.map());
                break;
            case R.id.btn_array://array type
                L.e(Data.array());
                break;
            case R.id.btn_json://json data
                L.i(new Gson().toJson(Data.array()));
                break;
        }
    }
```
![](https://github.com/ymex/cute.L/blob/master/app.png)

- Base type
![](https://github.com/ymex/cute.L/blob/master/base.png)
- Object type
![](https://github.com/ymex/cute.L/blob/master/object.png)
- List type
![](https://github.com/ymex/cute.L/blob/master/list.png)
- Map type
![](https://github.com/ymex/cute.L/blob/master/map.png)
- Array type
![](https://github.com/ymex/cute.L/blob/master/array.png)
