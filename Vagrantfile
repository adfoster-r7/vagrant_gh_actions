Vagrant.configure('2') do |config|
    config.vm.box = 'StefanScherer/windows_2022'

    config.vm.define 'windows'

    # Prevent SharedFoldersEnableSymlinksCreate errors
    config.vm.synced_folder '.', '/vagrant', disabled: true

    config.winrm.transport = 'plaintext'
    config.winrm.basic_auth_only = true

    config.vm.provider 'virtualbox' do |v|
        # v.gui = ENV['CI']&.empty?
        v.gui = false
    end
end
