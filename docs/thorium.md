# How to install Thorium browser?

```pwsh
scoop install akrami/thorium-avx2
```

> ⚠️
> 
>  I use `--silent-debugger-extension-api` flag to suppress the warning popup that some extensions cause, such as user-agent extensions.
>
> If you do not want this, you can remove it from the [manifest](bucket/thorium-avx2.json) and the `Portable Registrator` configuration.

# How to Register Thorium as a Browser?

```pwsh
scoop install akrami/portable-registrator
```

Add this to the end of `Portable Registrator` config:

```ini
    <AppType>
      <Name>Thorium Web-Browser</Name>
      <OpenParameters>--user-data-dir="%USERPROFILE%\scoop\apps\thorium-avx2\current\User Data" --silent-debugger-extension-api -url "%1"</OpenParameters>
      <FileAssociations>
        <string>.svg</string>
        <string>.pdf</string>
        <string>.htm</string>
        <string>.html</string>
        <string>.shtml</string>
        <string>.xht</string>
        <string>.xhtml</string>
      </FileAssociations>
      <URLAssociations>
        <string>http</string>
        <string>https</string>
        <string>ftp</string>
      </URLAssociations>
    </AppType>
```

<img width="1108" height="607" alt="image" src="https://github.com/user-attachments/assets/dec6d0fd-918a-4650-8b81-632cdb8505ce" />

# How to Make Thorium the Default Browser

Go to "Default apps" by [clicking here](ms-settings:defaultapps?registeredAppMachine=Thorium%20Portable), and then click "Set default."

<img width="1436" height="825" alt="image" src="https://github.com/user-attachments/assets/8fa613cf-22d8-444a-b32c-19b8b0f3eb7e" />

