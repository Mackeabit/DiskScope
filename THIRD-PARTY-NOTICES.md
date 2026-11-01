# Third-party components

The MIT license in LICENSE applies to original DiskScope code and artwork. Third-party components retain their own terms; they are not relicensed under the DiskScope license.

Windows App SDK and signed Win2D NuGet binaries use Microsoft Software License Terms. Their upstream source MIT licenses do not replace the binary terms. Object-code redistribution with DiskScope is permitted subject to the full component terms, including downstream protections and publisher obligations. See [binary terms](BINARY-TERMS.txt) and the [review and provenance](licenses/SUPPLEMENTAL.md).

This inventory includes build-time dependencies as well as runtime components. Some listed components are not used or copied into the application. No inference of runtime feature use should be made from a transitive package name.

| Component | Version | Package-declared license / notices |
| --- | --- | --- |
| CommunityToolkit.Mvvm | 8.4.2 | MIT · [text](licenses/CommunityToolkit.Mvvm/8.4.2/License.md) |
| Microsoft.Graphics.Win2D | 1.4.0 | http://www.microsoft.com/web/webpi/eula/eula_win2d_10012014.htm · [archived Microsoft EULA](licenses/Microsoft.Graphics.Win2D/1.4.0/LICENSE.html), [readable text](licenses/Microsoft.Graphics.Win2D/1.4.0/LICENSE.txt), [provenance](licenses/Microsoft.Graphics.Win2D/1.4.0/provenance.json) |
| Microsoft.NETCore.App.Runtime.win-x64 | 10.0.14 | MIT · [text](licenses/Microsoft.NETCore.App.Runtime.win-x64/10.0.14/LICENSE.TXT), [text](licenses/Microsoft.NETCore.App.Runtime.win-x64/10.0.14/THIRD-PARTY-NOTICES.TXT) |
| Microsoft.Web.WebView2 | 1.0.3719.77 | LICENSE.txt · [text](licenses/Microsoft.Web.WebView2/1.0.3719.77/LICENSE.txt), [text](licenses/Microsoft.Web.WebView2/1.0.3719.77/NOTICE.txt) |
| Microsoft.Windows.AI.MachineLearning | 2.1.74 | license.txt · [text](licenses/Microsoft.Windows.AI.MachineLearning/2.1.74/license.txt) |
| Microsoft.Windows.SDK.BuildTools.MSIX | 1.7.251221100 | sdk_license.txt · [text](licenses/Microsoft.Windows.SDK.BuildTools.MSIX/1.7.251221100/NOTICE.txt), [text](licenses/Microsoft.Windows.SDK.BuildTools.MSIX/1.7.251221100/sdk_license.txt) |
| Microsoft.Windows.SDK.BuildTools | 10.0.28000.2957 | https://aka.ms/WinSDKLicenseURL ·  |
| Microsoft.Windows.SDK.NET.Ref | 10.0.26100.57 | https://aka.ms/WinSDKLicenseURL ·  |
| Microsoft.WindowsAppSDK.AI | 2.5.5 | license.txt · [text](licenses/Microsoft.WindowsAppSDK.AI/2.5.5/license.txt) |
| Microsoft.WindowsAppSDK.Base | 2.0.4 | license.txt · [text](licenses/Microsoft.WindowsAppSDK.Base/2.0.4/license.txt), [text](licenses/Microsoft.WindowsAppSDK.Base/2.0.4/NOTICE.txt) |
| Microsoft.WindowsAppSDK.DWrite | 2.1.0 | license.txt · [text](licenses/Microsoft.WindowsAppSDK.DWrite/2.1.0/license.txt) |
| Microsoft.WindowsAppSDK.Foundation | 2.3.12 | license.txt · [text](licenses/Microsoft.WindowsAppSDK.Foundation/2.3.12/license.txt) |
| Microsoft.WindowsAppSDK.InteractiveExperiences | 2.1.9 | license.txt · [text](licenses/Microsoft.WindowsAppSDK.InteractiveExperiences/2.1.9/license.txt) |
| Microsoft.WindowsAppSDK.ML | 2.1.94 | license.txt · [text](licenses/Microsoft.WindowsAppSDK.ML/2.1.94/license.txt) |
| Microsoft.WindowsAppSDK.Runtime | 2.5.1 | license.txt · [text](licenses/Microsoft.WindowsAppSDK.Runtime/2.5.1/license.txt), [text](licenses/Microsoft.WindowsAppSDK.Runtime/2.5.1/NOTICE.txt) |
| Microsoft.WindowsAppSDK.Search | 2.5.5 | license.txt · [text](licenses/Microsoft.WindowsAppSDK.Search/2.5.5/license.txt) |
| Microsoft.WindowsAppSDK.Widgets | 2.0.5 | license.txt · [text](licenses/Microsoft.WindowsAppSDK.Widgets/2.0.5/license.txt) |
| Microsoft.WindowsAppSDK.WinUI | 2.3.9 | license.txt · [text](licenses/Microsoft.WindowsAppSDK.WinUI/2.3.9/license.txt), [text](licenses/Microsoft.WindowsAppSDK.WinUI/2.3.9/NOTICE.txt), [text](licenses/Microsoft.WindowsAppSDK.WinUI/2.3.9/tools/NOTICE.txt) |
| Microsoft.WindowsAppSDK | 2.5.1 | license.txt · [text](licenses/Microsoft.WindowsAppSDK/2.5.1/license.txt), [text](licenses/Microsoft.WindowsAppSDK/2.5.1/NOTICE.txt) |
| System.Numerics.Tensors | 9.0.0 | MIT · [text](licenses/System.Numerics.Tensors/9.0.0/LICENSE.TXT), [text](licenses/System.Numerics.Tensors/9.0.0/THIRD-PARTY-NOTICES.TXT) |

## Bundled font

Pretendard Variable 1.3.9, copyright (c) 2021 Kil Hyung-jin, is bundled unmodified under the [SIL Open Font License 1.1](licenses/Pretendard/1.3.9/OFL.txt). The Reserved Font Name is Pretendard. The font retains its own license and is not relicensed under MIT. [Tagged source](https://github.com/orioncactus/pretendard/tree/v1.3.9) · [file provenance](licenses/Pretendard/1.3.9/provenance.json).

Win2D 1.4.0 declares a legacy Microsoft EULA URL and requires license acceptance; the package does not embed the terms. The original Microsoft document was recovered from an archived capture of that exact URL. The package-declared metadata above is retained unchanged. The archived terms are supplemental evidence, not a license file extracted from the package. See [provenance and conditions](licenses/SUPPLEMENTAL.md).

Generated by tools/collect-licenses.ps1 from the exact restored package inventory; -NoticesOnly refreshes this document from the saved inventory without restore or download. Local cache paths and package download metadata are intentionally omitted.
