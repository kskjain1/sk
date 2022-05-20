<script src="https://partial-honest1.cs159.force.com/WebSchedulevforcesite/lightning/lightning.out.js"></script>
 
    <div id="LightningAppDivId">
        <!-- Lightning Web Component will be included here. -->
    </div>
    
    <script>
 
    $Lightning.use(
        "c:schedulerApp", // Name of Aura Dependency app where c is namespace.
        function (
        ) { // Callback function
            $Lightning.createComponent(
                "c:showSlots", // Name of Lightning Component where c is namespace.
                { authToken :"6Cel800D7X0000008smQ8887X0000006xLo68s8aWNuDCQGH3qCysjOoWECcMQX7ZkQcJXOvl4CoylSp8AlvqH9MQAz67Yk7fhAm76dkYPe",
                    
                    serviceAppointmentId:'08p7X000000ZUxcQAG'
                }, // attribute parameters
                "LightningAppDivId", // Id of the element where Lightning Component will be rendered.
                function(cmp){
                    document.querySelector('c-show-slots').addEventListener("scheduledRecord", function (event) {
                        console.log('vf event data window listener => ', event.detail);
                    });
                }
            );
        },
'https://partial-honest1.cs159.force.com/WebSchedulevforcesite/'
    );
    </script>  
