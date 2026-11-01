# Supplemental license provenance — 2026-10-31

The inventory preserves the exact packages' declared metadata. Supplemental documents below do not replace or broaden a dependency's terms. Original DiskScope code and artwork remain MIT licensed.

## Win2D 1.4.0: binary terms recovered; redistribution is conditional

The signed `Microsoft.Graphics.Win2D` 1.4.0 NuGet package does **not** embed a license document. Its nuspec declares `requireLicenseAcceptance=true` and `http://www.microsoft.com/web/webpi/eula/eula_win2d_10012014.htm`. The live URL now redirects to an unrelated Windows development page. [NuGet license metadata](https://www.nuget.org/packages/Microsoft.Graphics.Win2D/1.4.0/License).

The original **Microsoft Software License Terms — Microsoft Win2D** were recovered from a [2025-03-13 capture of that exact Microsoft URL](https://web.archive.org/web/20250313073221/http://www.microsoft.com/web/webpi/eula/eula_win2d_10012014.htm). Included evidence:

- [Unmodified archived HTML](Microsoft.Graphics.Win2D/1.4.0/LICENSE.html), retaining its Windows-1252 encoding.
- [Readable UTF-8 transcription](Microsoft.Graphics.Win2D/1.4.0/LICENSE.txt), with only whitespace normalized; English and French text retained.
- [Version, URLs, SHA-256 hashes, signature result and DLL matches](Microsoft.Graphics.Win2D/1.4.0/provenance.json).

The [official package build script](https://github.com/microsoft/Win2D/blob/winappsdk/main/build/nuget/build-nupkg.cmd) deliberately selects this Microsoft EULA URL for signed Microsoft binary builds and the upstream MIT URL for other builds. The inspected script's Git blob is `fcf39290076ed5df85ee609d0d0965660ccf0353`. The local package passed `dotnet nuget verify --all` for Microsoft author and NuGet repository signatures. The two Win2D DLLs shipped with DiskScope match the package byte for byte. These checks establish package provenance, not a new grant of rights.

The recovered EULA provides a conditional object-code redistribution grant:

| EULA section | Requirement and DiskScope treatment |
| --- | --- |
| 2.a.i | Object code may be distributed with developed programs. DiskScope distributes the unmodified DLLs as part of its Windows application. |
| 2.a.ii | Add significant primary functionality and display a valid program copyright notice. DiskScope supplies the scanner, accounting, exploration UI and its own copyright notice. |
| 2.a.ii | Require distributors and external end users to agree to protective terms. [BINARY-TERMS.txt](../BINARY-TERMS.txt), the full component terms and the release download notice must accompany distribution. A notice file by itself does not establish legally effective assent in every jurisdiction. |
| 2.a.ii | The publisher must indemnify, defend and hold Microsoft harmless for the claims described in the clause. This obligation is not removed by using MIT for DiskScope or by including license files. |
| 2.a.iii | Preserve notices; distribute for Windows only; do not imply Microsoft endorsement; obey the remaining restrictions, including those on subjecting Microsoft code to an Excluded License. DiskScope does not relicense the Microsoft DLLs under MIT. |

Read the complete terms, including their scope, export, warranty, liability and regional provisions. The previous **missing-document blocker is resolved**; the conclusion is conditional redistribution permission, not an unconditional legal clearance or completed release certification. Windows App SDK has its own similar distribution requirements below.

### Source license and evidence limits

The [official upstream source license](https://github.com/microsoft/Win2D/blob/winappsdk/main/LICENSE.txt) is MIT; an unmodified copy is included as [Win2D-upstream-LICENSE.txt](supplemental/Win2D-upstream-LICENSE.txt). It must not be substituted for the signed NuGet binary terms.

The package's `Win2d.githash.txt` records `57e06e2c24703526f500035129251d063881a44d`, which could not be resolved in the public repository. No exact-source or reproducible-build claim is made. The EULA evidence comes from the package-declared URL and Microsoft's documented build selection, independently of that unresolved source revision.

A [Microsoft Q&A discussion](https://learn.microsoft.com/en-us/answers/questions/6050369/commercial-redistribution-license-for-microsoft-gr) supplied the archive location. Its volunteer moderator response is a discovery aid, not a publisher authorization. No direct confirmation was obtained from Microsoft; the primary evidence is the archived Microsoft document. This review covers version **1.4.0 only** and must be repeated if the package or declared terms change.

## Windows SDK BuildTools

The package declares <https://aka.ms/WinSDKLicenseURL>, which resolved to Microsoft's `sdk_license.rtf`. The unmodified [Windows-SDK-LICENSE.rtf](supplemental/Windows-SDK-LICENSE.rtf) is included. BuildTools is a build dependency; its tool executables are not distributed as part of DiskScope.

## Windows App SDK and .NET

The inventory includes notices from the exact restored packages, including Windows App SDK **2.5.1** and .NET runtime **10.0.14**. [Windows App SDK terms](Microsoft.WindowsAppSDK/2.5.1/LICENSE.txt) section 3.a.i permits redistribution of files binplaced by the package with an application, including self-contained deployment. Sections 3.b–3.c impose significant-functionality, downstream-protection, publisher-indemnity and other conditions; the indemnity clause contains an exception for claims based solely on unmodified distributable code. The complete terms control.

All package notices remain included. DiskScope's MIT license does not relicense third-party components. Compatibility and clean-machine readiness are separate from this license review.
