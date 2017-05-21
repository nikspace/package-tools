##composer.phar

1. install composer.phar
```
curl -sS https://getcomposer.org/installer | php
```
这个命令会将 composer.phar 下载到当前目录。PHAR（PHP 压缩包）是一个压缩格式，可以在命令行下直接运行。



2. 你可以使用 --install-dir 选项将 Composer 安装到指定的目录，例如：
```
curl -sS https://getcomposer.org/installer | php -- --install-dir=bin
```

当然也可以进行全局安装：
```
curl -sS https://getcomposer.org/installer | php
mv composer.phar /usr/local/bin/composer
```

在 Mac OS X 下也可以使用 homebrew 安装：
```
brew tap josegonzalez/homebrew-php
brew install josegonzalez/php/composer
```
不过通常情况下只需将 composer.phar 的位置加入到 PATH 环境变量就可以，不一定要全局安装。

3. edit composer.json 
```
{
    {
        "monolog/monolog": "1.2.*"
    }
}

```

4. install package dependency
```
php composer.phar install 
```

5. update dependency package 
```
php composer.phar update
```




