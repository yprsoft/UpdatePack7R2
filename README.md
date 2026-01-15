# 在Github Actions上使用UpdatePack7R2自动集成Windows 7更新

## 说明
1. 本项目的主要目的是使用UpdatePack7R2自动集成Windows 7 SP1更新(使用GithubActions自动构建)

## 地址
1. 本仓库地址: https://github.com/yuanpeirong/UpdatePack7R2 (只发布源码)
2. 备用仓库地址: https://github.com/yprsoft/UpdatePack7R2 (发布源码+镜像)
3. UpdatePack7R2地址: https://blog.simplix.info/update7/

## 版本说明

| 镜像名称 | 说明 | 映像数量 | 映像名称
| :----- | :----- | :----- | :-----
| install_Windows7x64ALL.wim | Windows 7 x64 SP1旗舰版+企业版 | 5个 | 家庭普通版、家庭高级版、专业版、旗舰版、企业版
| install_Windows7x64ULTIMATE.wim | Windows 7 x64 SP1旗舰版 | 4个 | 家庭普通版、家庭高级版、专业版、旗舰版
| install_Windows7x64ENTERPRISE.wim | Windows 7 x64 SP1企业版 | 1个 | 企业版
| install_Windows7x86ALL.wim | Windows 7 x86 SP1旗舰版+企业版 | 6个 | 简易版、家庭普通版、家庭高级版、专业版、旗舰版、企业版
| install_Windows7x86ULTIMATE.wim | Windows 7 x86 SP1旗舰版 | 5个 | 简易版、家庭普通版、家庭高级版、专业版、旗舰版
| install_Windows7x86ENTERPRISE.wim | Windows 7 x86 SP1企业版 | 1个 | 企业版
- 以上均为不带U版本，参考说明[https://bbs.pcbeta.com/viewthread-1976287-1-1.html](https://bbs.pcbeta.com/viewthread-1976287-1-1.html)

## 母盘信息
- `cn_windows_7_ultimate_with_sp1_x64_dvd_618537.iso`
- `cn_windows_7_enterprise_with_sp1_x64_dvd_620654.iso`
- `cn_windows_7_ultimate_with_sp1_x86_dvd_618763.iso`
- `cn_windows_7_enterprise_with_sp1_x86_dvd_620153.iso`

## 关于ISO镜像
- 本仓库只负责提供集成补丁后的wim镜像，需用户制作ISO文件(2026年1月最终版考虑提供)
- 如需制作ISO文件，可自行将下载下来的wim镜像，改名为`install.wim`，替换原版`旗舰版`或`企业版`镜像中的`install.wim`
- 若要显示`简易版(仅x86版本有)`、`家庭普通版`、`家庭高级版`、`专业版`，还需删除原版`旗舰版`镜像中的ei.cfg文件
- 若要集成`旗舰版+企业版`，还需要增加`install_Windows 7 ENTERPRISE.clg`文件(可从原版`企业版`镜像中提取)
