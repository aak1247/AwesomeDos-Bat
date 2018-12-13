# AwesomeDos-Bat
Some useful dos code


# code

## Unclassfied

### Get current path 获取当前路径

```dos
FOR /F %%i IN ('cd') DO @set CURRENT_PATH=%%i
echo %CURRENT_PATH%
```

### Traversing Fils in a folder 遍历文件夹下文件

```dos
set base_dir="c:\projects"
setlocal EnableDelayedExpansion
cd /d %base_dir%
for /r %base_dir%\folder1 %%I in (*.*) do (
    echo %%I
)

```

