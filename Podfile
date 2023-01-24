# Uncomment the next line to define a global platform for your project
platform :ios, ’13.0’

install! 'cocoapods', :deterministic_uuids => false

target 'test' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for test

pod 'SwiftyJSON'
pod 'SDWebImage'
pod 'KeychainSwift'
pod 'IQKeyboardManagerSwift'
pod 'SVProgressHUD'
pod 'SwiftyStoreKit'
pod "SwiftPhoneNumberFormatter"
pod 'ObjectMapper'
pod 'AlgoliaSearchClient', '~> 8.16'
pod 'ReachabilitySwift'

pod 'Firebase'
pod 'Firebase/Functions'
pod 'Firebase/Core'
pod 'Firebase/Storage'
pod 'Firebase/Auth'
pod 'Firebase/DynamicLinks'
pod 'Firebase/Messaging'
pod 'FirebaseAnalytics'
pod 'FirebaseCrashlytics'
pod 'Firebase/Installations'
pod 'Firebase/Database'

pod 'GoogleMaps'
pod 'GooglePlaces'
pod 'GoogleSignIn'
pod 'GoogleAnalytics'
pod 'Google-Mobile-Ads-SDK'
pod 'PersonalizedAdConsent'

post_install do |installer|

    installer.pods_project.targets.each do |target|
      if target.respond_to?(:product_type) and target.product_type == "com.apple.product-type.bundle"
        target.build_configurations.each do |config|
            config.build_settings['CODE_SIGNING_ALLOWED'] = 'NO'
        end
      end
    end

  end

end