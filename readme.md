Things to be done of we want to extract webpack.config.json file
1) add all file to git add . then git commit -m "any message" ----------------> theme thhere should not any modified filese , code must me update(fresh code)
2) then run these command i.e yarn run eject
3) then it will also for person , enter yes
4) then you will get a webpack.config.json file in the nodules_modules folders
5) then open that webpack.config.json file in the nodules_modules folders then 
6)  // devtool: isEnvProduction
    //   ? shouldUseSourceMap
    //     ? 'source-map'
    //     : false
    //   : isEnvDevelopment && 'cheap-module-source-map',  -----> commmet these line (line no 135 to139 in webpack.config.json file) and
 add these line in our   webpack.config.json file   ---->  devtool: 'cheap-module-source-map',
7) then in webpack.config.json file
            sourceMap: isEnvProduction && shouldUseSourceMap, ---> comment these one at evry place where you see thesee 
            and
            replace these one with sourceMap: true
            
8) now you can see the .css,.scss,and js extact filese name and you can find the error where its in seeing it in the chrome console
           
            
            
            
