load(
    "@build_bazel_rules_swift//swift:swift.bzl",
    "swift_library",
)

load(
    "@build_bazel_rules_apple//apple:ios.bzl",
    "ios_application",
)

swift_library(
    name = "Sources",
    srcs = glob([
        "Sources/**/*.swift",
        "Resources/Config/Constants.swift",
        "Resources/Storyboards/Storyboards.swift",
    ]),
    data = glob([
        "CHMeetupApp/Sources/**/*.xib",
        "CHMeetupApp/Resources/Storyboards/*.storyboard",
    ]),
    visibility = ["//visibility:public"],
    deps = [
        "//:Fabric",
        "//:Crashlytics",
        "//:Realm",
        "//:RealmSwift",
        "//:Kingfisher",
        "//:SVProgressHUD",
    ],
)

ios_application(
    name = "CHMeetupApp",
    resources = glob([
        "Resources/Assets/Assets.xcassets/**",
        "Resources/Assets/Colors.xcassets/**",
    ]),
    entitlements = "CHMeetupApp.entitlements",
    strings = ["Resources/Localizations/Localizable.strings"],
    bundle_id = "CocoaHeads",
    families = [
        "iphone",
    ],
    infoplists = ["Resources/Config/Info.plist"],
    minimum_os_version = "11.0",
    visibility = ["//visibility:public"],
    deps = [
        ":Sources",
    ],
)
