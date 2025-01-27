## Exercise 3b: Build an Open AI application with Python

1. Search and select **Azure Synapse Analytics** in the Azure portal.

      ![](images/p2.png)

1.  On the **Overview** blade under the **Getting started** section, click **Open** to open Synapse Studio.
     
    ![](images/open-workspace.png)
    
1. Click on **Develop (1)**, then click on **+ (2)**, and select **Import**.

    ![](images/import-note.png)

1. Navigate to the `C:\labfile\OpenAIWorkshop\scenarios\powerapp_and_python\python` location and select `OpenAI_notebook.ipynb`, then click on **Open**.

     ![](images/notebook.png)

1. Select **openaisparkpool** from the drop-down menu of **Attach to**.

    ![](images/openai-sparkpool.png)

1. Run the notebook step-by-step to complete this exercise. Click on the **Run** button next to the cell.

     ![](images/run.png)

1. In **1. Install OpenAI**, click on the **Run** button next to the first cells, and click on the **stop session**. Please wait till **Apache Spark pools** turn to stop state. 

     ![](images/run-python1.png)

      > **Note**: you may need to restart the kernel to use updated packages

1. In **2. Import helper libraries and instantiate credentials**, and replace the **AZURE_OPENAI_API_KEY** and **AZURE_OPENAI_ENDPOINT** with your API key and endpoint URL.

    ![](images/key-endpoint.png)
   
From Azure Portal, navigate to the **openaicustom-<inject key="openaimodulename" enableCopy="true"/>** resource group, and select the Azure OpenAI resource.

    ![](images/Ex4b-S7.1.png)

Under Resource Management, select **Keys and Endpoint (1)**, and click **Show Keys (2)**. Copy **Key 1 (3)** and **Endpoint (4)**, and replace the **AZURE_OPENAI_API_KEY** and **AZURE_OPENAI_ENDPOINT** with your API key and Endpoint URL in the script.

   ![](images/p22.png)
     
    > **Note:** If you encounter an error "Openai module not found", enter `%` in before the **pip install** in the Install OpenAI cell and re-run the notebook again.

1. For **2. Choose a Model**, replace the **model** value from **text-curie-001** to **demomodel**.

    ![](images/choosemodel.png)

1. In **temperature**, replace **engine** value from **text-curie-001** to **demomodel**.

     ![](images/temp.png)

1. In **top_p**, replace **engine** value from **text-curie-001** to **demomodel**.

     ![](images/top-p.png)

1. For **n**, replace **engine** value from **text-curie-001** to **demomodel**.

     ![](images/n.png)

1. In **logprobs**, replace **engine** value from **text-curie-001** to **demomodel**.

     ![](images/logprobs.png)

1. After running the notebook successfully, click on **Publish all**.

     ![](images/publish.png)

1. Then click on **Publish** to save the changes. 

    ![](images/publish-1.png)
