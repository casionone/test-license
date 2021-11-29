## 相关链接

**linkis svn源码和安装包**
https://dist.apache.org/repos/dist/dev/incubator/linkis/1.0.3-RC1/

**linkis maven仓库staging地址**
https://repository.apache.org/content/repositories/orgapachelinkis-1048

**linkis snapshot 包地址** 
https://repository.apache.org/content/groups/snapshots/org/apache/linkis/

**linkis 1.0.3版本release notes** 
https://github.com/apache/incubator-linkis/issues/1110

**发布流程梳理** https://github.com/casionone/incubator-linkis/blob/for-test/apache-release-linkis.md

## 发起投票

> Linkis 仍在孵化阶段，需要进行两次投票

- Linkis社区投票，发送邮件至：`dev@linkis.apache.org`
- incubator社区投票，发送邮件至：`general@incubator.apache.org` Linkis毕业后，只需要在Linkis社区投票

### Linkis 社区投票阶段

1. Linkis社区投票，发起投票邮件到`dev@linkis.apache.org`。PMC需要先按照文档检查版本的正确性，然后再进行投票。 经过至少72小时并统计到3个`+1 PMC member`票后，即可进入下一阶段的投票。
2. 宣布投票结果,发起投票结果邮件到`dev@linkis.apache.org`。

#### Linkis社区投票模板

```html

邮件内容

```html
标题：
[VOTE] Release Apache Linkis (Incubating) 1.0.3-RC1

内容：

Hello Apache Linkis PPMC and Community,

    This is a call for vote to release Apache Linkis (Incubating) version 1.0.3

    Release notes:
	https://github.com/apache/incubator-linkis/issues/1110

    The release candidates:
    	https://dist.apache.org/repos/dist/dev/incubator/linkis/1.0.3-RC1

    Maven artifacts are available in a staging repository at:
	https://repository.apache.org/content/repositories/orgapachelinkis-1048

    Git tag for the release:
	https://github.com/apache/incubator-linkis/tree/1.0.3-RC1

    Keys to verify the Release Candidate:
	https://dist.apache.org/repos/dist/dev/incubator/linkis/KEYS

    This has been signed with PGP key 557A529D205AFE73D1FC7C48DCF229EF6FD6D28C, corresponding to peacewong@apache.org.

    The vote will be open for at least 72 hours or until necessary number of votes are reached.

    Please vote accordingly:

	[ ] +1 approve

	[ ] +0 no opinion

	[ ] -1 disapprove with the reason

    Checklist for reference:

	[ ] Download links are valid.

	[ ] Checksums and PGP signatures are valid.

	[ ] Source code distributions have correct names matching the current release.

	[ ] LICENSE and NOTICE files are correct for each Linkis repo.

	[ ] All files have license headers if necessary.

	[ ] No compiled archives bundled in source archive.

    More detail checklist  please refer:
	https://cwiki.apache.org/confluence/display/INCUBATOR/Incubator+Release+Checklist

Thanks,
Shuai Di
```

