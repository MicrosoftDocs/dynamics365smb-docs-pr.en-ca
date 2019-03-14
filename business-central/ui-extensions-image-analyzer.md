---
title: Using the Image Analyzer Extension | Microsoft Docs
description: This extensions lets you analyse images of contact persons and items to find attributes, so you can quickly assign them in Business Central.
documentationcenter: 
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: API, extension, Cognitive Services, image, computer vision, attribute, tag, recognition
ms.date: 10/01/2018
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: caf7cf5afe370af0c4294c794c0ff9bc8ff4c31c
ms.openlocfilehash: 803d755a7caa470b97bf606f0f8916d0135d047e
ms.contentlocale: en-ca
ms.lasthandoff: 11/22/2018

---

# <a name="the-image-analyzer-extension"></a><span data-ttu-id="f681f-103">The Image Analyzer Extension</span><span class="sxs-lookup"><span data-stu-id="f681f-103">The Image Analyzer Extension</span></span>
<span data-ttu-id="f681f-104">The Image Analyzer extension uses powerful image analytics provided by the Computer Vision API for Microsoft Cognitive Services to detect attributes in the images that you import for items and contact persons, so you can easily review and assign them.</span><span class="sxs-lookup"><span data-stu-id="f681f-104">The Image Analyzer extension uses powerful image analytics provided by the Computer Vision API for Microsoft Cognitive Services to detect attributes in the images that you import for items and contact persons, so you can easily review and assign them.</span></span> <span data-ttu-id="f681f-105">For items, attributes could be whether the item is a table or a car, and whether it is red or blue.</span><span class="sxs-lookup"><span data-stu-id="f681f-105">For items, attributes could be whether the item is a table or a car, and whether it is red or blue.</span></span> <span data-ttu-id="f681f-106">For contact persons, attributes can be gender or age.</span><span class="sxs-lookup"><span data-stu-id="f681f-106">For contact persons, attributes can be gender or age.</span></span>

<span data-ttu-id="f681f-107">Image Analyzer suggests attributes based on tags that the Computer Vision API finds, and a confidence level.</span><span class="sxs-lookup"><span data-stu-id="f681f-107">Image Analyzer suggests attributes based on tags that the Computer Vision API finds, and a confidence level.</span></span> <span data-ttu-id="f681f-108">By default, it suggests attributes only if it is at least 80% sure that the attribute is correct.</span><span class="sxs-lookup"><span data-stu-id="f681f-108">By default, it suggests attributes only if it is at least 80% sure that the attribute is correct.</span></span> <span data-ttu-id="f681f-109">You can set another confidence level, if needed.</span><span class="sxs-lookup"><span data-stu-id="f681f-109">You can set another confidence level, if needed.</span></span> <span data-ttu-id="f681f-110">To learn more about how the tags and confidence level are determined, see [Computer Vision API](https://go.microsoft.com/fwlink/?linkid=851476).</span><span class="sxs-lookup"><span data-stu-id="f681f-110">To learn more about how the tags and confidence level are determined, see [Computer Vision API](https://go.microsoft.com/fwlink/?linkid=851476).</span></span>  

<span data-ttu-id="f681f-111">Image Analyzer is free in [!INCLUDE[d365fin](includes/d365fin_md.md)], but there is a limit to the number of items that you can analyze during a certain period of time.</span><span class="sxs-lookup"><span data-stu-id="f681f-111">Image Analyzer is free in [!INCLUDE[d365fin](includes/d365fin_md.md)], but there is a limit to the number of items that you can analyze during a certain period of time.</span></span> <span data-ttu-id="f681f-112">By default, you can analyse 100 images per month.</span><span class="sxs-lookup"><span data-stu-id="f681f-112">By default, you can analyze 100 images per month.</span></span>

<span data-ttu-id="f681f-113">After you enable the extension, Image Analyzer runs each time you import an image to an item or contact person.</span><span class="sxs-lookup"><span data-stu-id="f681f-113">After you enable the extension, Image Analyzer runs each time you import an image to an item or contact person.</span></span> <span data-ttu-id="f681f-114">You will see the attributes, confidence level, and details right away, and can decide what to do with each attribute.</span><span class="sxs-lookup"><span data-stu-id="f681f-114">You will see the attributes, confidence level, and details right away, and can decide what to do with each attribute.</span></span> <span data-ttu-id="f681f-115">If you imported images before you enabled the Image Analyzer extension, you must go to the item or contact cards and choose the **Analyze Picture** action.</span><span class="sxs-lookup"><span data-stu-id="f681f-115">If you imported images before you enabled the Image Analyzer extension, you must go to the item or contact cards and choose the **Analyze Picture** action.</span></span>  

## <a name="privacy-notice"></a><span data-ttu-id="f681f-116">Privacy Notice</span><span class="sxs-lookup"><span data-stu-id="f681f-116">Privacy Notice</span></span>
<span data-ttu-id="f681f-117">This extension uses the Computer Vision API from Microsoft Cognitive Services, which may have varying levels of compliance commitments than [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="f681f-117">This extension uses the Computer Vision API from Microsoft Cognitive Services, which may have varying levels of compliance commitments than [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="f681f-118">When you enable the Image Analyzer extension, Customer Data such as a contact image or an item image will be sent to the Computer Vision API.</span><span class="sxs-lookup"><span data-stu-id="f681f-118">When you enable the Image Analyzer extension, Customer Data such as a contact image or an item image will be sent to the Computer Vision API.</span></span> <span data-ttu-id="f681f-119">By installing this extension you agree for this limited set of data to be sent to the Computer Vision API.</span><span class="sxs-lookup"><span data-stu-id="f681f-119">By installing this extension you agree for this limited set of data to be sent to the Computer Vision API.</span></span> <span data-ttu-id="f681f-120">Note that you may disable, as well as uninstall, the Image Analyzer extension at any time to discontinue use of this functionality.</span><span class="sxs-lookup"><span data-stu-id="f681f-120">Note that you may disable, as well as uninstall, the Image Analyzer extension at any time to discontinue use of this functionality.</span></span> <span data-ttu-id="f681f-121">For more information, see [Microsoft Trust Center](https://go.microsoft.com/fwlink/?linkid=851463).</span><span class="sxs-lookup"><span data-stu-id="f681f-121">For more information, see [Microsoft Trust Center](https://go.microsoft.com/fwlink/?linkid=851463).</span></span>

## <a name="requirements"></a><span data-ttu-id="f681f-122">Requirements</span><span class="sxs-lookup"><span data-stu-id="f681f-122">Requirements</span></span>
<span data-ttu-id="f681f-123">There are a few requirements for the images:</span><span class="sxs-lookup"><span data-stu-id="f681f-123">There are a few requirements for the images:</span></span>

* <span data-ttu-id="f681f-124">Image formats: JPEG, PNG, GIF, BMP</span><span class="sxs-lookup"><span data-stu-id="f681f-124">Image formats: JPEG, PNG, GIF, BMP</span></span>  
* <span data-ttu-id="f681f-125">Maximum file size: Less than 4 MB</span><span class="sxs-lookup"><span data-stu-id="f681f-125">Maximum file size: Less than 4 MB</span></span>  
* <span data-ttu-id="f681f-126">Image dimensions: Greater than 50 x 50 pixels</span><span class="sxs-lookup"><span data-stu-id="f681f-126">Image dimensions: Greater than 50 x 50 pixels</span></span>  

## <a name="to-enable-image-analyzer"></a><span data-ttu-id="f681f-127">To enable Image Analyzer</span><span class="sxs-lookup"><span data-stu-id="f681f-127">To enable Image Analyzer</span></span>
<span data-ttu-id="f681f-128">The Image Analyzer extension is built-in to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="f681f-128">The Image Analyzer extension is built-in to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="f681f-129">You just need to turn it on.</span><span class="sxs-lookup"><span data-stu-id="f681f-129">You just need to turn it on.</span></span>

> [!NOTE]  
> <span data-ttu-id="f681f-130">To enable the Image Analyzer extension, you must be an administrator.</span><span class="sxs-lookup"><span data-stu-id="f681f-130">To enable the Image Analyzer extension, you must be an administrator.</span></span> <span data-ttu-id="f681f-131">Make sure that you are assigned the **SUPER** user permission set.</span><span class="sxs-lookup"><span data-stu-id="f681f-131">Make sure that you are assigned the **SUPER** user permission set.</span></span>

1. <span data-ttu-id="f681f-132">To enable the Image Analyzer extension, do one of the following:</span><span class="sxs-lookup"><span data-stu-id="f681f-132">To enable the Image Analyzer extension, do one of the following:</span></span>

* <span data-ttu-id="f681f-133">Open an item or contact card.</span><span class="sxs-lookup"><span data-stu-id="f681f-133">Open an item or contact card.</span></span> <span data-ttu-id="f681f-134">In the notification bar, choose **Analyze Images**, and then follow the steps in the assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="f681f-134">In the notification bar, choose **Analyze Images**, and then follow the steps in the assisted setup guide.</span></span>  
* <span data-ttu-id="f681f-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Connections**, and then choose **Image Analysis Setup**.</span><span class="sxs-lookup"><span data-stu-id="f681f-135">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Connections**, and then choose **Image Analysis Setup**.</span></span> <span data-ttu-id="f681f-136">Choose the **Enable Image Analyzer** check box, and then complete the steps in the assisted setup guide.</span><span class="sxs-lookup"><span data-stu-id="f681f-136">Choose the **Enable Image Analyzer** check box, and then complete the steps in the assisted setup guide.</span></span>  

    > [!TIP]  
    > <span data-ttu-id="f681f-137">The **Image Analysis Setup** page is also where you can change the degree of confidence for attribute suggestions.</span><span class="sxs-lookup"><span data-stu-id="f681f-137">The **Image Analysis Setup** page is also where you can change the degree of confidence for attribute suggestions.</span></span> <span data-ttu-id="f681f-138">For example, if you want to require a greater degree of confidence, you can enter a higher percentage.</span><span class="sxs-lookup"><span data-stu-id="f681f-138">For example, if you want to require a greater degree of confidence, you can enter a higher percentage.</span></span>

## <a name="to-analyze-an-image-of-an-item"></a><span data-ttu-id="f681f-139">To analyse an image of an item</span><span class="sxs-lookup"><span data-stu-id="f681f-139">To analyze an image of an item</span></span>
<span data-ttu-id="f681f-140">The following steps describe how to analyse an image that was imported before you enabled the Image Analyser extension.</span><span class="sxs-lookup"><span data-stu-id="f681f-140">The following steps describe how to analyze an image that was imported before you enabled the Image Analyzer extension.</span></span>  

1. <span data-ttu-id="f681f-141">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f681f-141">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f681f-142">Choose the item, and then choose the **Analyze Picture** action.</span><span class="sxs-lookup"><span data-stu-id="f681f-142">Choose the item, and then choose the **Analyze Picture** action.</span></span>  
3. <span data-ttu-id="f681f-143">The **Image Analyzer Attributes** page displays the detected attributes, the confidence level, and other details about the attribute.</span><span class="sxs-lookup"><span data-stu-id="f681f-143">The **Image Analyzer Attributes** page displays the detected attributes, the confidence level, and other details about the attribute.</span></span> <span data-ttu-id="f681f-144">Use the **Action to perform** options to specify what to do with the attribute.</span><span class="sxs-lookup"><span data-stu-id="f681f-144">Use the **Action to perform** options to specify what to do with the attribute.</span></span>  

    > [!TIP]  
    > <span data-ttu-id="f681f-145">You can add the name of the attribute to the item description by choosing **Add to item description**.</span><span class="sxs-lookup"><span data-stu-id="f681f-145">You can add the name of the attribute to the item description by choosing **Add to item description**.</span></span> <span data-ttu-id="f681f-146">For example, this can be useful for quickly adding detail.</span><span class="sxs-lookup"><span data-stu-id="f681f-146">For example, this can be useful for quickly adding detail.</span></span>  

## <a name="to-analyze-a-picture-of-a-contact-person"></a><span data-ttu-id="f681f-147">To analyse a picture of a contact person</span><span class="sxs-lookup"><span data-stu-id="f681f-147">To analyze a picture of a contact person</span></span>
<span data-ttu-id="f681f-148">The following steps describe how to analyse an image that was imported before you enabled the Image Analyser extension.</span><span class="sxs-lookup"><span data-stu-id="f681f-148">The following steps describe how to analyze an image that was imported before you enabled the Image Analyzer extension.</span></span>  

1. <span data-ttu-id="f681f-149">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Contacts**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f681f-149">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Contacts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f681f-150">Choose the contact person, and then choose the **Analyze Picture** action.</span><span class="sxs-lookup"><span data-stu-id="f681f-150">Choose the contact person, and then choose the **Analyze Picture** action.</span></span>  
3. <span data-ttu-id="f681f-151">On the **Profile Questionnaire** FastTab, review the suggestions, and make corrections if needed.</span><span class="sxs-lookup"><span data-stu-id="f681f-151">On the **Profile Questionnaire** FastTab, review the suggestions, and make corrections if needed.</span></span>  

## <a name="blacklisting-suggested-attributes"></a><span data-ttu-id="f681f-152">Blacklisting suggested attributes</span><span class="sxs-lookup"><span data-stu-id="f681f-152">Blacklisting suggested attributes</span></span>
<span data-ttu-id="f681f-153">If the analysis suggests an attribute that you do not want to see you can blacklist the attribute.</span><span class="sxs-lookup"><span data-stu-id="f681f-153">If the analysis suggests an attribute that you do not want to see you can blacklist the attribute.</span></span> <span data-ttu-id="f681f-154">Use caution, however.</span><span class="sxs-lookup"><span data-stu-id="f681f-154">Use caution, however.</span></span> <span data-ttu-id="f681f-155">Blacklisted attributes are not suggested for other items or contact persons either.</span><span class="sxs-lookup"><span data-stu-id="f681f-155">Blacklisted attributes are not suggested for other items or contact persons either.</span></span> <span data-ttu-id="f681f-156">If you regret blacklisting an attribute, you can choose **Blacklisted Attributes**, and then delete the attribute from the list.</span><span class="sxs-lookup"><span data-stu-id="f681f-156">If you regret blacklisting an attribute, you can choose **Blacklisted Attributes**, and then delete the attribute from the list.</span></span>

## <a name="to-use-your-own-account-for-the-computer-vision-api"></a><span data-ttu-id="f681f-157">To use your own account for the Computer Vision API</span><span class="sxs-lookup"><span data-stu-id="f681f-157">To use your own account for the Computer Vision API</span></span>
<span data-ttu-id="f681f-158">You can also use your own account for the Computer Vision API, for example, if you want to analyse more images than we allow.</span><span class="sxs-lookup"><span data-stu-id="f681f-158">You can also use your own account for the Computer Vision API, for example, if you want to analyze more images than we allow.</span></span>  

1. <span data-ttu-id="f681f-159">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Image Analyzer Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f681f-159">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Image Analyzer Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f681f-160">Enter the **API URI** and **API Key** that you received for Computer Vision API.</span><span class="sxs-lookup"><span data-stu-id="f681f-160">Enter the **API URI** and **API Key** that you received for Computer Vision API.</span></span>  

    > [!NOTE]  
    > <span data-ttu-id="f681f-161">You must add **/analyze** at the end of the API URI, if it isn't already there.</span><span class="sxs-lookup"><span data-stu-id="f681f-161">You must add **/analyze** at the end of the API URI, if it isn't already there.</span></span> <span data-ttu-id="f681f-162">For example: ```https://cronus.api.cognitive.microsoft.com/vision/v1.0/analyze```.</span><span class="sxs-lookup"><span data-stu-id="f681f-162">For example: ```https://cronus.api.cognitive.microsoft.com/vision/v1.0/analyze```.</span></span>

## <a name="to-see-how-many-analyses-you-have-left-in-the-current-period"></a><span data-ttu-id="f681f-163">To see how many analyses you have left in the current period</span><span class="sxs-lookup"><span data-stu-id="f681f-163">To see how many analyses you have left in the current period</span></span>
<span data-ttu-id="f681f-164">You can view the number of analyses you've done, and how many you can still do, in the current period.</span><span class="sxs-lookup"><span data-stu-id="f681f-164">You can view the number of analyses you've done, and how many you can still do, in the current period.</span></span>  

1. <span data-ttu-id="f681f-165">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Image Analyzer Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="f681f-165">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Image Analyzer Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f681f-166">The **Limit type**, **Limit value**, and **Analyzes performed** provide the usage information.</span><span class="sxs-lookup"><span data-stu-id="f681f-166">The **Limit type**, **Limit value**, and **Analyzes performed** provide the usage information.</span></span>  

## <a name="to-stop-using-the-image-analyzer-extension"></a><span data-ttu-id="f681f-167">To stop using the Image Analyzer extension</span><span class="sxs-lookup"><span data-stu-id="f681f-167">To stop using the Image Analyzer extension</span></span>
1. <span data-ttu-id="f681f-168">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Connections**, and then choose **Image Analyzer Setup**.</span><span class="sxs-lookup"><span data-stu-id="f681f-168">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Connections**, and then choose **Image Analyzer Setup**.</span></span>  
2. <span data-ttu-id="f681f-169">Clear the **Enable Image Analyzer** check box.</span><span class="sxs-lookup"><span data-stu-id="f681f-169">Clear the **Enable Image Analyzer** check box.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f681f-170">See Also</span><span class="sxs-lookup"><span data-stu-id="f681f-170">See Also</span></span>
[<span data-ttu-id="f681f-171">Work with Item Attributes</span><span class="sxs-lookup"><span data-stu-id="f681f-171">Work with Item Attributes</span></span>](inventory-how-work-item-attributes.md)  
<span data-ttu-id="f681f-172">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="f681f-172">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
[<span data-ttu-id="f681f-173">Getting Started</span><span class="sxs-lookup"><span data-stu-id="f681f-173">Getting Started</span></span>](product-get-started.md)  
