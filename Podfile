# Uncomment the next line to define a global platform for your project
platform :ios, '11.0'

source 'https://github.com/CocoaPods/Specs.git'

target 'ActionSample' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

  # Pods for ActionSample
  pod 'SnapKit', '~> 4.0'

  target 'ActionSampleTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'ActionSampleUITests' do
    # Pods for testing
  end

end

post_install do |installer_representation|
  installer_representation.pods_project.targets.each do |target|
      target.build_configurations.each do |config|
          config.build_settings.delete 'IPHONEOS_DEPLOYMENT_TARGET'
      end
  end
end