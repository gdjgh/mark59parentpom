````markdown
# Mark59 Parent POM

A parent POM for Mark59 Java projects, published to JitPack for easy consumption by child projects.

## Quick Start - Using This Parent POM

Add this to your `pom.xml`:

```xml
<repositories>
    <repository>
        <id>jitpack.io</id>
        <url>https://jitpack.io</url>
    </repository>
</repositories>

<parent>
    <groupId>com.github.gdjgh</groupId>
    <artifactId>mark59-parent-pom</artifactId>
    <version>5.6.3.00</version>
</parent>
```

**No authentication required** ✅

---

## Managed Dependencies

This parent POM provides versions for:

- **Apache JMeter**: 5.6.3
- **Mark59 Scripting**: 6.5
- **Mark59 DataHunter API**: 6.5
- **Log4j 2**: 2.25.4
- **Batik**: 1.17
- **XStream**: 1.4.21
- **DataFaker**: 2.5.4

### Compiler Configuration
- **Java Version**: 17
- **Source Encoding**: UTF-8

---

## Publishing Releases

### Prerequisites
- You have push access to this repository
- GitHub Actions is enabled

### To Create a Release

1. Go to **Actions** tab in GitHub
2. Select **"Create Release for JitPack"** workflow
3. Click **"Run workflow"**
4. Enter the version (e.g., `5.6.3.01`)
5. (Optional) Add release notes
6. Click **"Run workflow"**

### What Happens Automatically
- POM version is updated
- Maven build is verified
- Changes are committed to main
- Git tag is created (v5.6.3.01)
- GitHub Release is created
- **JitPack automatically builds and publishes** the package

### Monitor the Build
Visit: `https://jitpack.io/#gdjgh/mark59parentpom/5.6.3.01`

---

## Version History

See [Releases](https://github.com/gdjgh/mark59parentpom/releases) for all published versions.

---

## FAQ

### Q: Do I need to authenticate to use this parent POM?
**A:** No! JitPack provides public, unauthenticated access to all builds.

### Q: How do I use a specific version?
**A:** Update the version in the `<parent>` tag:
```xml
<version>5.6.3.01</version>
```

You can use any Git tag from the repository (see Releases).

### Q: Can I use SNAPSHOT versions?
**A:** Yes! Use `main-SNAPSHOT` to build from the latest main branch:
```xml
<version>main-SNAPSHOT</version>
```

### Q: What if JitPack fails to build?
**A:** Check the build log at `https://jitpack.io/` - it's usually a Maven configuration issue that appears in the logs.

---

## License

Apache License 2.0

## Repository

- **GitHub**: https://github.com/gdjgh/mark59parentpom
- **JitPack**: https://jitpack.io/#gdjgh/mark59parentpom
````
