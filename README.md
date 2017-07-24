# oceattworkspace
1. Go to the cloned repository in local
Eg : C:\Installables\oceattworkspace\oceattworkspace

2. Create a new module from the Archetype : 
mvn archetype:generate  -DarchetypeGroupId=com.att.oce -DarchetypeArtifactId=oce-minishift-archetype -DarchetypeVersion=1.0-SNAPSHOT -DgroupId=com.att.oce -DartifactId=testocenew

3. Checkin the new module into git
git add <moduleNme>
git commit -m "first commit"
git push -u origin master

4. Run the OC Create command to create the pipleline
oc create -f <gitURL>/pipeline.yml
