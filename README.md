# Web Application Security Lab Portfolio

Documented web-security exercises by **Lewis Joseph Feik**, focused on understanding vulnerable application behavior and explaining the evidence collected in a training environment.

The current repository is a collection of **DVWA lab write-ups and screenshots**. It gives visitors a route through the documented exercises, their stated observations, and the security concepts each exercise illustrates.

## Lab directory

| Lab | What the existing write-up documents | Evidence |
|---|---|---|
| [Stored cross-site scripting](Cross-Site-Scripting/dvwa-stored-xss-lab-master/README.md) | Stored input executing as JavaScript, persistence across page refreshes, and the risk of exposing browser-accessible session data. | [Screenshots](Cross-Site-Scripting/dvwa-stored-xss-lab-master/screenshots/) |
| [Insecure file upload](File-Upload-Exploitation/dvwa-file-upload-lab-master/README.md) | Uploading executable content in a deliberately vulnerable application and observing server-side command execution. | [Screenshots](File-Upload-Exploitation/dvwa-file-upload-lab-master/screenshots/) |
| [Legacy mixed lab archive](SQL-Injection/dvwa-stored-xss-lab/README.md) | A larger historical collection whose README currently describes file-upload/RCE work and whose screenshots cover several lab steps. | [Screenshots](SQL-Injection/dvwa-stored-xss-lab/screenshots/) |

**Directory naming note:** the legacy archive lives under `SQL-Injection`, but its current README is titled "DVWA File Upload → Remote Code Execution (RCE)." The path is preserved so existing links keep working. Its folder name alone should not be treated as evidence of a completed SQL-injection exercise.

## What to look for

- **Objective:** the application behavior being investigated.
- **Method:** the controlled steps recorded in the individual lab.
- **Observation:** the page, output, or screenshot supporting a conclusion.
- **Impact and remediation:** why the behavior matters and what a defensive fix would need to address.

The existing lab notes identify **Kali Linux in UTM, Apache, PHP, and DVWA** as their environment. The repository's present contents support these documented exercises; they do not establish a broader tool assessment or a production penetration test.

## Reading and reproducing

Start with a linked lab README, then compare its stated result with its supporting screenshots. This repository does not include an application runtime, dependency manifest, or automated test suite; the vulnerable training application must be supplied separately.

```bash
git clone https://github.com/FeikL2002/Web-App-Penetration-Testing.git
cd Web-App-Penetration-Testing
```

Reproduction belongs in a local training environment or a system whose owner has explicitly authorized testing. Keep DVWA and other intentionally vulnerable applications isolated from public access. Published screenshots are historical evidence rather than a fresh verification of a running target.

## Portfolio context

These exercises support my study of web application security, Linux command-line work, evidence collection, and technical reporting. The root index explains the material currently committed; individual lab write-ups retain their original detail and context.

- [Hocking College coursework and reference notes](https://github.com/FeikL2002/HockingCollege)
- [Software and engineering projects](https://github.com/FeikL2002/Engineered-Solutions-self-made-)

## License

See [LICENSE](LICENSE). Bundled materials and third-party software retain their respective notices and terms.
