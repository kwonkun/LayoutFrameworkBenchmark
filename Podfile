source 'https://cdn.cocoapods.org/'

use_frameworks!

project 'LayoutFrameworkBenchmark.xcodeproj'

platform :ios, '10.0'

inhibit_all_warnings!

post_install do |installer|
    installer.generated_projects.each do |project|
        project.targets.each do |target|
            target.build_configurations.each do |config|
                config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '13.0'
            end
        end
    end
end

target 'LayoutFrameworkBenchmark' do
    pod 'FlexLayout'
    pod 'LayoutKit', :git => 'https://github.com/LinkedInAttic/LayoutKit.git'
    pod 'NotAutoLayout'
    pod 'NKFrameLayoutKit'
    pod 'PinLayout'
    pod 'Texture'

    pod 'Reveal-SDK'
end
