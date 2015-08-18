workspace 'ProjectABWorkspace'
use_frameworks!

def ios_platform
  platform :ios, '8.0'
end

def mac_platform
  platform :osx, '10.9'
end

def my_shared_pods
  pod 'INTUGroupedArray', '~> 1.0'
end

xcodeproj 'ProjectA/ProjectA'
target 'ProjectA-iOS' do
  xcodeproj 'ProjectA/ProjectA'
  link_with 'ProjectA-iOS'
  ios_platform
  my_shared_pods
end
target 'ProjectA-Mac' do
  xcodeproj 'ProjectA/ProjectA'
  link_with 'ProjectA-Mac'
  mac_platform
  my_shared_pods
end

xcodeproj 'ProjectB/ProjectB'
target 'ProjectB-iOS' do
  xcodeproj 'ProjectB/ProjectB'
  link_with 'ProjectB-iOS'
  ios_platform
  my_shared_pods
end
target 'ProjectB-Mac' do
  xcodeproj 'ProjectB/ProjectB'
  link_with 'ProjectB-Mac'
  mac_platform
  my_shared_pods
end
