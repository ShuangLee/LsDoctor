platform:ios,'8.0'
inhibit_all_warnings!
use_frameworks!
project 'LsDoctor/LsDoctor.xcodeproj'

def pods

pod 'SnapKit', '~> 3.0.2'
pod 'SVProgressHUD', '~> 1.1.3'
pod 'Kingfisher'
pod 'YYKit'

end

target 'LsDoctor' do
    pods
end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['SWIFT_VERSION'] = '3.0'
        end
    end
end
