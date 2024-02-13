 - task: ArchiveFiles@2
    displayName: 'Create project zip'
    inputs:
      rootFolderOrFile: '$(Build.SourcesDirectory)/rr-cxp-logicapp/project_output/src/logicApp'
      includeRootFolder: false
      archiveType: 'zip'
      archiveFile: '$(Build.SourcesDirectory)/rr-cxp-logicapp/project_output/$(Build.BuildId).zip'
      replaceExistingArchive: true