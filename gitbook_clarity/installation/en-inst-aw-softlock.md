---
description: "EN INST A+W Softlock"
---



# EN INST A+W Softlock

 Dongle News
 Jürgen Makowka
 Pohlheim, January 19, 2018




Software
 Softwarefor
          forGlass
              Glassand
                    andWindows
                        Windows
 Bedenket, worum Ihr bittet …




           Bedenket worum Ihr bittet,

        Es könnte Euch gewährt werden




© A+W                    2
 Be Careful What You Wish For




    Be careful what you wish for,
    for the gods may grant you!


                     Marion Zimmer Bradley: “The Mists of Avalon”


© A+W                     3
 What’s New?
 ■ ‘Softlocks’ supported
   ‒ Gemalto Sentinel Software Licenses

 ■ Improved requesting of license files
   ‒ Website for requesting license files




        ‒ New administration tools for Internal Sales

© A+W                                        4
 A+W Softlock Basics
 ■ Gemalto Sentinel Software License combined with the A+W License Server
        ‒   Gemalto <swallowed> SafeNet <swallowed> Aladdin <swallowed> Fast


 ■ A Softlock has an A+W Dongle no
   ‒ Number range 1000000 to 8999999

 ■ A Softlock is bound to its physical or virtual machine
   ‒ ‘Fingerprint’ of the machine must be collected
      • Initial installation only!
   ‒ License file creation requires the fingerprint (unless the softlock is known)

 ■ Creating a softlock with a fingerprint causes expenses for A+W
        ‒   Creating a softlock is about as expensive as buying a new hardware dongle


 ■ Softlocks cannot be recycled
   ‒ They can be re-located to another machine (‘Rehosting’)
© A+W                                            5
 A+W Softlock Advantages & Disadvantages
 ■ Advantages
   ‒ No hardware module
          •   No shipment required
          •   Cannot break
          •   Cannot get lost
          •   Doesn’t require USB over LAN connection when used in datacenter
          •   Can be used in cloud (Azure, AWS)


 ■ Disadvantages
   ‒ No hardware module
          •   No sticker, dongle no cannot be easily identified
        ‒ More cumbersome handling
          •   Requires fingerprint collection before license file creation
          •   Cannot be moved easily from one machine to another
          •   License update may require additional steps
        ‒ Less secure
          •   Not bound to hardware (not even the host machine’s)



© A+W                                             6
 A+W Softlock Workflow (First Installation)
 ■      IP* requests compilation of license (from dongle@a-w.com), based on a PO+
        ‒ (Some head start appreciated)
 ■      Internal Sales compiles the license and assigns a new A+W Softlock no
        ‒ The license, together with the A+W Softlock no is stored in a database

 ■      At installation time IP makes sure the target machine is in its final state
        ‒ Final machine name
        ‒ Final domain membership
        ‒ Final DNS properties
 ■      IP installs the ‘SoftlockPreparePackage’ on the target machine
        ‒   \\jupiter\Doku_DocuWare\AWEnterprise\LicenseServer\!General\FAQ_Tips_Tricks\Softlock\SoftlockPreparePackage.zip

 ■      IP collects the target machine’s fingerprint
 ■      IP uses https://www.a-w.com/licenseprovider to download license file
        ‒ Fingerprint enters here
 ■      IP installs A+W License Server on target machine, using downloaded license file

 * IP = Installing Person

 + PO = Purchase order




© A+W                                                                7
 A+W Softlock After Installation
 ■      Critical changes (virtual machines, may invalidate A+W Softlock)
        ‒ Rename computer (does always invalidate)
        ‒ Change computer’s domain membership
        ‒ Change computer’s DNS environment (may include ip address of DNS server)

 ■      Non-critical changes (virtual machines)
        ‒ Change Memory
        ‒ Change no of processor cores
        ‒ Migrate VM within the same network
        ‒ Change ‘physical’ network adapter
        ‒ Change ‘physical’ disk

 ■      More restrictive checks can be imposed on VMs, but are not by default


 ■      Different with physical machines
        ‒ Avoid to change any hardware component

© A+W                                          8
 A+W Softlock Initial Installation (Demo)




 ■Demo
© A+W                      9
 A+W Softlock Initial Installation (More Info)


 ■ The fingerprint can be sent to dongle@a-w.com. Internal Sales will send back
   the license file.
   ‒ There are possible delays because of time zone differences and office
       hours



 ■ Reading Material
   ‒ \\jupiter\Doku_DocuWare\AWEnterprise\LicenseServer\!General\FAQ_Tips
     _Tricks\Softlock
   ‒ General hints for using A+W Softlocks (PDF file)
   ‒ Checklist for installing an A+W Softlock (PDF file)




© A+W                                   10
 A+W Softlock License Update Workflow
 ■ IP request license modification (from dongle@a-w.com), based on PO
 ■ Internal Sales modifies license and stores the result


 ■ At installation time IP uses https://www.a-w.com/licenseprovider to download
   the new license
   ‒ Multiple options, depending on situation

 ■ IP uses ‘A+W LicenseServices Config Tool’ to activate the new license




© A+W                                    11
 A+W Softlock License Update (Demo)




 ■Demo
© A+W                  12
 A+W Softlock Update (Things to Know)
 ■ A+W Softlock updates have a precise order
   ‒ An update targeted to a different value of the update counter cannot be
     activated
           •   You cannot go back to an older license version just by re-installing the older
               license file
        ‒ An update can be activated only once

 ■ Update download options
   ‒ Standard (for most recent know value of UC)
   ‒ By UC value
   ‒ By A+W Softlock information file
   ‒ Previous license versions




© A+W                                             13
 A+W Softlock Activate Older License (Demo)




 ■Demo
© A+W                    14
 A+W LicenseProvider Web App (Things to Know)
 ■ Licenses can be downloaded for A+W Softlocks and A+W Dongles
 ■ Licenses cannot be downloaded for the older HARDLOCK (OEM license files)
 ■ Permission to use the A+W LicenseProvider Web App is maintained by ICT
   ‒ Permission is granted by the A+W departments’ directors
   ‒ Specific roles imply download permission
   ‒ Permission check is based on AWAGDOM group membership
 ■ The A+W LicenseProvider Web App does not (and will never) enable the user
   to change the contents of a license




© A+W                                  15
 Q&A




 ■Any questions so far?


© A+W       16
 A+W Softlock Move (Rehosting)
 ■ A+W Softlock can be moved from one machine to another
 ■ Softlock must be ‘rehostable’
   ‒ Internal Sales can prevent this when defining the license
   ‒ Whether or not a customer gets rehosting permission is decided by A+W
      management
   ‒ Default is that the A+W Softlock is rehostable
 ■ Moving requires that both machines are simultaneously available
   ‒ However, a direct connection is not required
 ■ The target machine of the move must be in its final state
 ■ The license can be moved along with the A+W Softlock
 ■ Moving is a multistep process
   ‒ The part pertaining to the Gemalto Sentinel Software License is called
     ‘Rehosting’




© A+W                                    17
 A+W Softlock Move Workflow
 ■      IP ascertains that target machine is in its final state
 ■      IP installs SoftlockPreparePackage on target machine
 ■      IP uses ‘A+W Softlock Tool’ to create .awtmid file
 ■      IP transfers .awtmid file to source machine

 ■      IP stops and disables A+W License Server on the source machine
 ■      IP uses ‘A+W Softlock Tool’ to remove A+W Softlock and create .awrhif file
        ‒ .awrhif may include the current license
        ‒ After this operation A+W License Server no longer works on source machine
        ‒ A+W License Server may be uninstalled at this time
 ■      IP transfers .awrhif file to target machine

 ■      IP uses ‘A+W Softlock Tool’ to install A+W Softlock on target machine
        ‒ License may be installed if it was included in the .awrhif
 ■      IP installs A+W License Server on target machine (unless already present)
 ■      IP optionally requests and installs new license (if license was not transferred)



© A+W                                            18
 A+W Softlock Move (Demo)




 ■Demo
© A+W                  19
 A+W License (Additional Information)
 ■      A+W Softlock live from February 12, 2018
 ■      Minimum requirements
        ‒ Gemalto Sentinel Runtime version 7.54 or above (‘A+W Distribution for Gemalto Sentinel
            Runtime’)
        ‒ A+W License Server version v6.4 with latest patches
            • Older license clients will work with that version

 ■      There are options for specific situations
        ‒ Options are always controlled by Internal Sales
        ‒ For virtual machines the A+W Softlock can be bound to the virtualization hardware
           • Prevents cloning
           • Failover and Migration not possible
        ‒ Moving the A+W Softlock can be prevented
           • Re-locating the A+W License Server to another machine requires a new A+W
                Softlock

 ■      There is a Dongle mode which is similar to the A+W Softlock
        ‒ Works with our standard dongles
        ‒ License updates bound to Update Counter as with the A+W Softlock


© A+W                                              20
 Q&A




 ■Any questions left?


© A+W      21
 The End




 ■Thank you for your patience!




© A+W          22

