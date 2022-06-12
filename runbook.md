## 使用可能なテンプレート一覧

```shell
dotnet new -l
```

## ソリューションファイルを作成

```shell
dotnet new sln
```

## web api を作成

```shell
dotnet new webapi -n API
```

##　クラスライプラリを作成

```shell
dotnet new classlib -n Application
dotnet new classlib -n Domain
dotnet new classlib -n Persistence
```

## ソリューションにプロジェクトを追加

```shell
dotnet sln add API/API.csproj
dotnet sln add Application
dotnet sln add Domain
donnet sln add Persistence
```

## ソリューション内のプロジェクトを確認

```shell
dotnet sln list
```

## 参照の追加

```shell
cd API
dotnet add reference ../Application
cd Application
dotnet add reference ../Persistence
dotnet add reference ../Domain
cd Persistence
dotnet add reference ../Domain
```
