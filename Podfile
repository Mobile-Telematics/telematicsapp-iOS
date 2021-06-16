source 'https://github.com/CocoaPods/Specs.git'

platform :ios, '10.0'
inhibit_all_warnings!
use_frameworks!

def available_pods
    pod 'RaxelPulse'
    pod 'HEREMaps'
    pod 'Firebase/Core'
    pod ‘Firebase/Database’
    pod 'Firebase/Auth'
    pod 'Firebase/Storage'
    #pod 'FirebaseUI/Database'
    pod 'AFNetworking'
    pod 'JSONModel'
    pod 'CocoaLumberjack/Swift', '3.5.3'
    pod 'SDWebImage', '5.9.0'
    pod 'GKImagePicker@robseward'
    pod 'SystemServices'
    pod 'KVNProgress'
    pod 'UICountingLabel'
    pod 'UIActionSheet+Blocks'
    pod 'UIAlertView+Blocks'
    pod 'CMTabbarView', '0.2.0'
    pod 'Charts', '3.3.0'
    pod 'YYWebImage'
    pod 'SHSPhoneComponent'
    pod "IQDropDownTextField"
    pod "RMessage"
    pod 'MagicalRecord', :git => 'https://github.com/magicalpanda/MagicalRecord'
    pod "IQMediaPickerController"
    pod 'libPhoneNumber-iOS', '~> 0.8'
    pod 'KDLoadingView'
    pod 'ImagePicker', '3.1.0'
    pod 'CircleTimer', '0.2.0'
end


target 'TelematicsApp' do
    available_pods
end


post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['DEBUG_INFORMATION_FORMAT'] = 'dwarf'
        end
        target.build_configurations.each do |config|
            config.build_settings['CLANG_WARN_OBJC_IMPLICIT_RETAIN_SELF'] = 'NO'
        end
    end
end
