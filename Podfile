
source 'https://github.com/CocoaPods/Specs.git'

platform :ios, '10.0'
use_frameworks!

target "ExampleTDD" do
    
    def testing_pods
        pod 'Quick'
        pod 'Nimble'
    end

    target 'ExampleTDDTests' do
        testing_pods
    end

    target 'ExampleTDDUITests' do
        testing_pods
    end

end


post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['SWIFT_VERSION'] = '4.0'
        end
    end
end

