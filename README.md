# nuvo_p_series_home_assistant
NuVo P Series Home Assistant


import upnpclient
import json

#~ devices = upnpclient.discover()

#~ print (devices[0])

d = upnpclient.Device("http://192.168.1.34:52657/00000000-0000-0000-0000-0025ed1cb9c8.xml")

zone_memberid = d.ZoneService.GetMemberID()
zone_memberid = zone_memberid["MemberID"]
print (zone_memberid)
#~ print ('{"memberIDs":["' + zone_memberid + '"]}')
#~ print (d.ZoneService.GroupCreate(memberIDs ='{"memberIDs":["' + zone_memberid + '"]}'))


#~ print (d.ZoneService.UserTap())


d = upnpclient.Device("http://192.168.1.26:60707/00000000-0000-0000-0000-0025ed1cbac3.xml")

zone_memberid2 = d.ZoneService.GetMemberID()
zone_memberid2 = zone_memberid2["MemberID"]
print (zone_memberid2)

#~ print (d.ZoneService.GroupMemberSetGroup(memberIDs='["'+zone_memberid+'"]', groupID='gid6KwTOCqwtrWXSqJM'))



#--------------------

#Works
#~ print (d.ZoneService.GroupCreate(memberIDs='["'+zone_memberid+'" , "'+zone_memberid2+'"]'))




#~ print (d.AVTransport.SetAVTransportURI(InstanceID='0',CurrentURI='nuvo:pandora:StationList/station_4536940277391457006', CurrentURIMetaData='0'))





#--------------------------
#~ print (d.AVTransport.GetMediaInfo(InstanceID = '0'))
#~ print("")
#~ print (d.AVTransport.GetTransportInfo(InstanceID = '0'))
#~ print("")
#~ print (d.AVTransport.GetPositionInfo(InstanceID = '0'))
#~ print("")
#~ print (d.AVTransport.Pause(InstanceID = '0'))
#~ print("")
#~ print (d.AVTransport.GetDeviceCapabilities(InstanceID = '0'))
#~ print("")
#~ print (d.AVTransport.GetTransportSettings(InstanceID = '0'))
#~ print("")

#~ http://192.168.1.33:58887/00000000-0000-0000-0000-0025ed1c1ef2.xml

#~ argsdef_in
#~ print ("Services")
#~ print (d.services)

#~ print ""

#~ for device in devices:
	#~ if((device.friendly_name.find("NuVo Zone")) != -1):
		#~ print (device.friendly_name)
		#~ print (device.location)
		
		#~ zone_get = device.ZoneService.Get()
		#~ print (zone_get["Title"])


#~ zone_get = d.ZoneService.Get()
	#~ print (zone_get["Title"])
	#~ print ("")





































#~ print "AVTransport Actions"
#~ print d.AVTransport.actions
#~ print ""


#~ print "Rendering Actions"
#~ print d.RenderingControl.actions
#~ print ""

#~ print "ConnectionManager Actions"
#~ print d.ConnectionManager.actions
#~ print ""

#~ print "ContentDir Actions"
#~ print d.ContentDirectory.actions
#~ print ""




#~ print d.ZoneService.Get()


#~ print d.ZoneService.GetActive()

#~ d = upnpclient.Device("http://192.168.1.31:48127/00000000-0000-0000-0000-0025ed1c1f17.xml")

#~ print "Services"
#~ print d.services

#~ print ""

#~ print "Zones Actions"
#~ print d.ZoneService.actions
#~ print ""

#~ print "AVTransport Actions"
#~ print d.AVTransport.actions
#~ print ""


#~ print "Rendering Actions"
#~ print d.RenderingControl.actions
#~ print ""

#~ print "ConnectionManager Actions"
#~ print d.ConnectionManager.actions
#~ print ""

#~ print "ContentDir Actions"
#~ print d.ContentDirectory.actions
#~ print ""




#~ print d.ZoneService.Get()



#~ print d.ZoneService.GetActive()



