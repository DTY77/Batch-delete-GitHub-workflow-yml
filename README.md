# -workflows-yml-
一、创建批量删除workflows的yml文件
进入.github→workflows→Add file→Create new file，我这里随便命名的001.yml。然后填入仓库名中为“模板”的内容。


retain_days举例比如填1，就把昨天之前的记录都删了。
keep_minimum_runs则字面意思想要保留的记录条数。
上述文件里repository里的用户名/仓库名记得替换到你自己的。
提前把GITHUB_TOKEN填入仓库Settings里的Secrets环境变量里。


以下是申请GitHub访问令牌（Access Token）的步骤：
登录到您的GitHub帐户。
点击右上角的头像，然后选择 "Settings"（设置）。
在左侧导航栏中，选择 "Developer settings"（开发者设置）。
在 "Developer settings" 页面上，选择 "Personal access tokens"（个人访问令牌）。
在 "Personal access tokens" 页面上，点击 "Generate new token"（生成新令牌）按钮。
提供一个描述以标识该访问令牌的用途。
在 "Select scopes"（选择范围）部分，选择要授予该令牌的权限。这些权限将决定该访问令牌可以执行哪些操。请根据您的需求选择合适的权限，例如 repo（仓库），admin:org（组织管理）等。
完成设置后，点击页面底部的 "Generate token"（生成令牌）按钮。
生成的访问令牌将显示在屏幕上，请确保复制该令牌并妥善保存。一旦离开该页面，您将无法再次查看完整的访问令牌。


二、Run这个配置文件的Action
All workflows下选择autodelete然后点击Run Workflow,自动执行删除，开始批量处理。
