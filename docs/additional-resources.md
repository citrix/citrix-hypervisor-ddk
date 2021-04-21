# Additional Resources

In addition to supplemental packs, a variety of mechanisms are available
for partners to interface with Citrix Hypervisor, and add value to the user
experience. This chapter overviews the mechanisms, and provides web
links to further information.

If pack authors have any questions concerning what should (or should
not) be included in a pack, or how a particular customization goal might
be achieved, they are encouraged to contact their Citrix technical
account manager.

## Xen API plug-ins

Whilst the Xen API provides a wide variety of calls to interface with
Citrix Hypervisor, partners have the opportunity to add to the API by means of
XAPI plug-ins. These consist of Python scripts that are installed as
part of supplemental packs, that can be run by using the
`host.call_plugin` XAPI call. These plug-ins can perform arbitrary
operations, including running commands in dom0, and making further XAPI
calls, using the XAPI Python language bindings.

For examples of how XAPI plug-ins can be used, please see the example
plug-ins in the `/etc/xapi.d/plugins/` directory of a standard Citrix Hypervisor
installation.

## XenCenter plug-ins

XenCenter plug-ins provides the facility for partners to add new menus
and tabs to the XenCenter administration GUI. In particular, new tabs
can have an embedded web browser, meaning that existing web-based
management interfaces can easily be displayed. When combined with Xen
API plug-ins to drive new menu items, this feature can be used by
partners to integrate features from their supplemental packs into one
centralized management interface for Citrix Hypervisor.

To learn how to create plug-ins for XenCenter, see the samples and accompanying
documentation in the [XenCenter Plug-in Specification and Examples](https://github.com/xenserver/xencenter-samples)
repository. The [Citrix XenCenter Plug-in Specification Guide](https://developer-docs.citrix.com/projects/xencenter-plugin-specification/en/latest/)
is available on the [Developer Documentation site](https://developer-docs.citrix.com/).

## Citrix Hypervisor SDK

The Xen API is a Remote Procedure Call (RPC) based API providing programmatic
access to the extensive set of Citrix Hypervisor management features and tools.
Although it is possible to write applications that use the API directly through
raw RPC calls, the task of developing third-party applications is greatly
simplified by using language bindings exposing the individual API calls as
first-class functions in the target language. The Citrix Hypervisor SDK provides
language bindings for the C, C#, Java, Python, and PowerShell programming languages.

The Citrix Hypervisor SDK is shipped as a set of compiled libraries and source
code, which include a class for every API class and a method for each API call.
The libraries are accompanied by a number of test programs that can be used as
pedagogical examples. The Citrix Hypervisor SDK can be downloaded from
<https://www.citrix.com/downloads/citrix-hypervisor/>.

The [Citrix Hypervisor Management API Reference](https://developer-docs.citrix.com/projects/citrix-hypervisor-management-api/en/latest/)
and the [Citrix Hypervisor Software Development Kit Guide](https://developer-docs.citrix.com/projects/citrix-hypervisor-sdk/en/latest/)
are available on the [Developer Documentation site](https://developer-docs.citrix.com/).
