# MandatoryTextInputLayoutV2

<p align="center">
  <img src="https://github.com/gzeinnumer/MandatoryTextInputLayoutV2/blob/master/preview/example1.jpg"/>
</p>

#
- gradle
```gradle
dependencies {
  ...
  implementation 'com.google.android.material:material:1.2.1'
}
```

- View
```xml
<com.google.android.material.textfield.TextInputLayout
    android:id="@+id/ed_p"
    style="@style/MyTextInputLayoutOutlinedBox.Man"
    android:layout_margin="16dp"
    android:layout_marginTop="16dp"
    app:suffixText="KM">

    <com.google.android.material.textfield.TextInputEditText
        android:id="@+id/ed"
        style="@style/MyTextInputEditText"
        android:hint="Kilometer sebelumnya"
        android:inputType="number" />

</com.google.android.material.textfield.TextInputLayout>
```

- Style
```xml
<style name="MyTextInputLayoutOutlinedBox" parent="Widget.MaterialComponents.TextInputLayout.OutlinedBox">
    <item name="android:layout_width">match_parent</item>
    <item name="android:layout_height">wrap_content</item>
    <item name="android:layout_marginTop">10dp</item>
</style>

<style name="MyTextInputLayoutOutlinedBox.Man">
    <!--        <item name="helperText">*Required</item>-->
    <item name="android:textColorHint">@color/my_mtrl_indicator_text_color</item>
    <!--        <item name="boxStrokeColor">@color/my_mtrl_outlined_stroke_color</item>-->
    <!--        <item name="helperTextTextColor">@color/my_mtrl_indicator_helper_text_color</item>-->
</style>

<style name="MyTextInputEditText">
    <item name="android:layout_width">match_parent</item>
    <item name="android:layout_height">wrap_content</item>
    <item name="android:alpha">1</item>
    <item name="android:textColor">@color/text_content</item>
</style>
```

- [res/values/color.xml](https://github.com/gzeinnumer/MandatoryTextInputLayoutV2/blob/master/app/src/main/res/values/colors.xml)
- [res/color/my_mtrl_indicator_text_color.xml](https://github.com/gzeinnumer/MandatoryTextInputLayoutV2/blob/master/app/src/main/res/color/my_mtrl_indicator_helper_text_color.xml)
- [res/color/my_mtrl_outlined_stroke_color.xml](https://github.com/gzeinnumer/MandatoryTextInputLayoutV2/blob/master/app/src/main/res/color/my_mtrl_outlined_stroke_color.xml)
- [res/color/my_mtrl_indicator_helper_text_color.xml](https://github.com/gzeinnumer/MandatoryTextInputLayoutV2/blob/master/app/src/main/res/color/my_mtrl_indicator_helper_text_color.xml)

---

```
Copyright 2021 M. Fadli Zein
```
