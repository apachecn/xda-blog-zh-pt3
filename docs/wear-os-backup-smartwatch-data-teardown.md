# 谷歌可能很快会让你在换到新手机时备份你的 Wear OS 智能手表数据

> 原文：<https://www.xda-developers.com/wear-os-backup-smartwatch-data-teardown/>

谷歌似乎正在努力解决 Wear OS 智能手表最令人讨厌的问题之一。Google Play 服务 v22.32.12 测试版中的新字符串显示，该公司可能很快会让用户在切换到新手机时选择备份他们的智能手表数据。

APK 拆卸通常可以预测应用程序未来更新中可能出现的功能，但我们在这里提到的任何功能都可能不会出现在未来的版本中。这是因为这些特性目前还没有在实时构建中实现，并且可能会被开发人员在未来的构建中随时引入。

目前，当你用新设备设置 Wear OS 智能手表时，你必须在工厂重置它。虽然有一种变通方法可以让你[将你的 Wear OS 智能手表与一部新手机配对，而无需重置它](https://www.xda-developers.com/pair-android-wear-without-factory-reset/)，但现在是时候谷歌为用户提供备份他们智能手表数据的选项，以使这个过程更加无缝。以下字符串表明该公司正在努力实现这一目标，备份 Wear OS 智能手表数据的能力可能会在不久的将来推出。

```
 <string name="companion_backup_opt_in_title">Back up your device with Google One</string>
<string name="companion_backup_settings_title">Backup by Google One</string>
<string name="companion_set_backup_account_title">Choose backup account</string> 
```

Google Play Services v22.32.12 测试版还包括关于即将到来的备份功能的新活动，进一步揭示了它将是一个选择加入的功能。

```
 <activity android:enabled="true" android:exported="true" android:icon="@drawable/APKTOOL_DUMMY_9ea" android:label="@string/companion_backup_opt_in_title" android:name="com.google.android.gms.wearable.backup.phone.BackupOptInActivity" android:process="@string/common_ui_process" android:theme="@style/common.Theme.GoogleSettings">
<intent-filter>
<action android:name="com.google.android.gms.wearable.COMPANION_BACKUP_OPT_IN"/>
<category android:name="android.intent.category.DEFAULT"/>
</intent-filter>
</activity>

<activity android:enabled="true" android:exported="true" android:icon="@drawable/APKTOOL_DUMMY_9ea" android:label="@string/companion_backup_settings_title" android:name="com.google.android.gms.wearable.backup.phone.BackupSettingsActivity" android:process="@string/common_ui_process" android:theme="@style/common.Theme.GoogleSettings">
<intent-filter>
<action android:name="com.google.android.gms.wearable.COMPANION_BACKUP_SETTINGS"/>
<category android:name="android.intent.category.DEFAULT"/>
</intent-filter>
</activity>

<activity android:enabled="true" android:exported="false" android:label="@string/companion_set_backup_account_title" android:name="com.google.android.gms.wearable.backup.phone.SetBackupAccountActivity" android:process="@string/common_ui_process" android:theme="@style/SudAlertDialogTheme.Light"/> 
```

每个活动也有新的布局，称为 companion _ backup _ opt _ in _ activity . XML、companion _ backup _ settings _ activity . XML 和 companion_account_activity.xml，但是，这些布局目前是空的。

备份 Wear OS 智能手表数据的能力将使切换到新手机更加无缝。但我们可能需要等待一段时间，因为它似乎还处于发展的早期阶段。我们会尽快让你知道我们即将推出的功能的更多细节。