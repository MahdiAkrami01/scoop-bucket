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

<img width="1119" height="652" alt="image" src="https://github.com/user-attachments/assets/b48a5b06-c410-4e4c-91c6-15c2eed4580b" />

# How to Make Thorium the Default Browser

- Press `Win+R` to open `Run`.
- Type `ms-settings:defaultapps?registeredAppMachine=Thorium%20Portable` and press Enter.
- Click "Set default".

<img width="1436" height="825" alt="image" src="https://github.com/user-attachments/assets/8fa613cf-22d8-444a-b32c-19b8b0f3eb7e" />

