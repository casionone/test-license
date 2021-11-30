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




### Step1 发起准备发布新版本的讨论

> 发起准备发布linkis-1.0.3版本的的DISCUSS讨论邮件到`dev@linkis.apache.org` ，说明本次发布的大体内容，由谁负责本次的release manager。

```html
标题：
[DISCUSS] Releasing Apache Linkis (Incubating) 1.0.3

内容：

Hello Apache Linkis PPMC and Community,

About three months to prepare, we are about to release a new version of Linkis-1.0.3.
We had an discussion[1] about this version two month ago, and carried out a series of preparations and tests before the release of the version.
And I would like to be the release manager this time.


The release note can be found here[2].
And I also create a new tag 1.0.3-RC1 for this release[3]


If you have any comments, welcome to discuss. If there is no question, I will start a vote a few day later.


[1] https://lists.apache.org/thread/c48z5r9726kv4x4hmhgq14ddsp25dftz
[2] https://github.com/apache/incubator-linkis/issues/1110
[3] https://github.com/apache/incubator-linkis/tree/1.0.3-RC1

Thanks,
Shuai Di

```
### Step2 发起RC版本的Linkis社区投票

- 最终的ASF正式版本前，可以进行多次RC版本发布和投票。对于最终的正式版本，在Linkis社区投票成功后，还需要发起incubator社区投票。
- PMC需要先按照文档检查版本的正确性，然后再进行投票。 
- 如果本次版本是作为正式版本发布，则经过至少72小时并统计到3个`+1 PMC member`票后，才可进入下一阶段的incubator社区投票。


```html

邮件内容

```html
标题：
[VOTE] Release Apache Linkis (Incubating) 1.0.3-RC1

内容：

Hello Apache Linkis PPMC and Community,

    This is a call for vote to release Apache Linkis (Incubating) version 1.0.3-RC1

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

投票后结束后，需要统计发布投票结果，并发送投票结果邮件


#### 发起incubator社区投票(正式ASF版本)
- Linkis社区投票成功之后，才能进行这一步
- incubator社区投票，发送邮件至：`general@incubator.apache.org`

```html
标题：
[VOTE] Release Apache Linkis(Incubating) ${release_version} ${rc_version}

内容：

Hello Incubator Community,

    This is a call for a vote to release Apache Linkis(Incubating) version
    ${release_version} ${rc_version}

    The Apache Linkis community has voted on and approved a proposal to release
    Apache Linkis(Incubating) version ${release_version} ${rc_version}

    We now kindly request the Incubator PMC members review and vote on this
    incubator release.

    Linkis community vote thread:
    • [投票链接]

    Vote result thread:
    • [投票结果链接]

    The release candidate:
    • https://dist.apache.org/repos/dist/dev/incubator/linkis/${release_version}-${rc_version}/

    Git tag for the release:
    • https://github.com/apache/incubator-linkis/releases/tag/${release_version}-${rc_version}

    Release notes:
    • https://github.com/apache/incubator-linkis/releases/tag/${release_version}-${rc_version}

    The artifacts signed with PGP key [填写你个人的KEY], corresponding to [填写你个人的邮箱], that can be found in keys file:
    • https://downloads.apache.org/incubator/linkis/KEYS

    The vote will be open for at least 72 hours or until necessary number of votes are reached.

    Please vote accordingly:

    [ ] +1 approve
    [ ] +0 no opinion
    [ ] -1 disapprove with the reason

Thanks,
On behalf of Apache Linkis(Incubating) community
```


