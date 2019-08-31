# Uncomment the next line to define a global platform for your project
platform :ios, '11.0'

# Ignore all warnings from pods
inhibit_all_warnings!

# Ignore warning from specific pod
# pod 'Realm', :inhibit_warnings => true

def common_pods
  pod 'SwiftUtilityKit', '0.1.1'
  pod 'Kingfisher', '5.7.0'
  pod 'SnapKit', '5.0.0'
  pod 'Then', '2.5.0'
  pod 'RxSwift', '5.0.0'
  pod 'RxCocoa', '5.0.0'
  pod 'Alamofire', '4.8.2'
end

def common_pods_for_test
  pod 'Quick', '2.1.0'
  pod 'Nimble', '8.0.1'
end

def common_pods_for_analyze
  pod 'SwiftLint', '0.31.0'
  pod 'CocoaAnalyzer', '0.4.6'
end

target 'BaseProject' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!
  common_pods
  common_pods_for_analyze
end

target 'BaseProjectTests' do
  common_pods_for_test
end

target 'BaseProjectUITests' do
  common_pods_for_test
end
