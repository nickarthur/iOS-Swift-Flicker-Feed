platform :ios, '8.0'
use_frameworks!

def shared_pods
    pod 'PagingView'
    pod 'Alamofire'
    pod 'AlamofireObjectMapper', '~> 2.1'
	pod 'SDWebImage'
end

target 'FlickerFeed' do
   shared_pods
end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['SWIFT_VERSION'] = '2.3'
        end
    end
end