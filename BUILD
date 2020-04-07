load(
    "@build_bazel_rules_apple//apple/internal:apple_framework_import.bzl",
    "apple_dynamic_framework_import",
)

apple_dynamic_framework_import(
    name = "Fabric",
    framework_imports = glob(["Frameworks/Fabric.framework/**"]),
    visibility = ["//visibility:public"],
)

apple_dynamic_framework_import(
    name = "Crashlytics",
    framework_imports = glob(["Frameworks/Crashlytics.framework/**"]),
    visibility = ["//visibility:public"],
)

apple_dynamic_framework_import(
    name = "Realm",
    framework_imports = glob(["Carthage/Build/iOS/Realm.framework/**"]),
    visibility = ["//visibility:public"],
)

apple_dynamic_framework_import(
    name = "RealmSwift",
    framework_imports = glob(["Carthage/Build/iOS/RealmSwift.framework/**"]),
    visibility = ["//visibility:public"],
)

apple_dynamic_framework_import(
    name = "Kingfisher",
    framework_imports = glob(["Carthage/Build/iOS/Kingfisher.framework/**"]),
    visibility = ["//visibility:public"],
)

apple_dynamic_framework_import(
    name = "SVProgressHUD",
    framework_imports = glob(["Carthage/Build/iOS/SVProgressHUD.framework/**"]),
    visibility = ["//visibility:public"],
)
