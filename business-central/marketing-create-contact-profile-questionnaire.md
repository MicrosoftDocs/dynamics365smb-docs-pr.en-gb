---
title: Use profiles to classify contacts
description: Set up profile questionnaires to help classify your business contacts
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: contacts, profiles
ms.author: edupont
ms.date: 04/01/2021
ms.openlocfilehash: 31321ce4cafd17efc8a7732c81e874df1a1d763a
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2021
ms.locfileid: "5785505"
---
# <a name="use-profile-questionnaires-to-classify-business-contacts"></a><span data-ttu-id="af454-103">Use Profile Questionnaires to Classify Business Contacts</span><span class="sxs-lookup"><span data-stu-id="af454-103">Use Profile Questionnaires to Classify Business Contacts</span></span>
<span data-ttu-id="af454-104">You can set up profile questionnaires that you want to use when entering information about your contacts' profiles.</span><span class="sxs-lookup"><span data-stu-id="af454-104">You can set up profile questionnaires that you want to use when entering information about your contacts' profiles.</span></span> <span data-ttu-id="af454-105">Within each questionnaire, you can set up the different questions you intend to ask your contacts.</span><span class="sxs-lookup"><span data-stu-id="af454-105">Within each questionnaire, you can set up the different questions you intend to ask your contacts.</span></span>  

<span data-ttu-id="af454-106">You can also run the questionnaire to answer some of the questions based on contact, customer, or vendor data automatically.</span><span class="sxs-lookup"><span data-stu-id="af454-106">You can also run the questionnaire to answer some of the questions based on contact, customer, or vendor data automatically.</span></span>  

## <a name="to-add-a-profile-questionnaire"></a><span data-ttu-id="af454-107">To add a profile questionnaire</span><span class="sxs-lookup"><span data-stu-id="af454-107">To add a profile questionnaire</span></span>
1.  <span data-ttu-id="af454-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Questionnaire Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="af454-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Questionnaire Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="af454-109">Choose the **New** Action.</span><span class="sxs-lookup"><span data-stu-id="af454-109">Choose the **New** Action.</span></span>  
3.  <span data-ttu-id="af454-110">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="af454-110">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-add-questions-to-a-profile-questionnaire"></a><span data-ttu-id="af454-111">To add questions to a profile questionnaire</span><span class="sxs-lookup"><span data-stu-id="af454-111">To add questions to a profile questionnaire</span></span>
1.  <span data-ttu-id="af454-112">Choose the relevant profile questionnaire, and then choose the **Edit Questionnaire Setup** action.</span><span class="sxs-lookup"><span data-stu-id="af454-112">Choose the relevant profile questionnaire, and then choose the **Edit Questionnaire Setup** action.</span></span>  
2.  <span data-ttu-id="af454-113">On the first empty line, in the **Type** field, choose **Question** and type your question in the **Description** field.</span><span class="sxs-lookup"><span data-stu-id="af454-113">On the first empty line, in the **Type** field, choose **Question** and type your question in the **Description** field.</span></span> <span data-ttu-id="af454-114">Fill in the other fields on this line.</span><span class="sxs-lookup"><span data-stu-id="af454-114">Fill in the other fields on this line.</span></span>  
3.  <span data-ttu-id="af454-115">On the next empty line, in the **Type** field, choose **Answer** and type your answer in the **Description** field.</span><span class="sxs-lookup"><span data-stu-id="af454-115">On the next empty line, in the **Type** field, choose **Answer** and type your answer in the **Description** field.</span></span>  
4.  <span data-ttu-id="af454-116">In the **Priority** field, select the priority.</span><span class="sxs-lookup"><span data-stu-id="af454-116">In the **Priority** field, select the priority.</span></span> <span data-ttu-id="af454-117">In the **From Value** and **To Value** fields, define a point range.</span><span class="sxs-lookup"><span data-stu-id="af454-117">In the **From Value** and **To Value** fields, define a point range.</span></span> <span data-ttu-id="af454-118">Contacts that receive points within the defined range will get the answer.</span><span class="sxs-lookup"><span data-stu-id="af454-118">Contacts that receive points within the defined range will get the answer.</span></span>  

<span data-ttu-id="af454-119">Repeat these steps to enter all the questions and answers within the profile questionnaire.</span><span class="sxs-lookup"><span data-stu-id="af454-119">Repeat these steps to enter all the questions and answers within the profile questionnaire.</span></span>

<span data-ttu-id="af454-120">After you have created a questionnaire, you must create contact ratings to classify your contacts.</span><span class="sxs-lookup"><span data-stu-id="af454-120">After you have created a questionnaire, you must create contact ratings to classify your contacts.</span></span> <span data-ttu-id="af454-121">You can also set up questions that are rated automatically based on information in the contact card.</span><span class="sxs-lookup"><span data-stu-id="af454-121">You can also set up questions that are rated automatically based on information in the contact card.</span></span>  

> [!NOTE]
> <span data-ttu-id="af454-122">If you enter a question that is automatically answered, choose <STRONG>Line</STRONG>, and then choose <STRONG>Question Details</STRONG>, to enter the criteria to automatically answer the question.</span><span class="sxs-lookup"><span data-stu-id="af454-122">If you enter a question that is automatically answered, choose <STRONG>Line</STRONG>, and then choose <STRONG>Question Details</STRONG>, to enter the criteria to automatically answer the question.</span></span>

## <a name="the-automatic-classification-of-contacts"></a><span data-ttu-id="af454-123">The Automatic Classification of Contacts</span><span class="sxs-lookup"><span data-stu-id="af454-123">The Automatic Classification of Contacts</span></span>
<span data-ttu-id="af454-124">You can automatically classify your contacts according to customer, vendor, and contact information, by setting up automatically answered profile questions on the **Profile Questionnaire Setup** page.</span><span class="sxs-lookup"><span data-stu-id="af454-124">You can automatically classify your contacts according to customer, vendor, and contact information, by setting up automatically answered profile questions on the **Profile Questionnaire Setup** page.</span></span>  

> [!NOTE]
> <span data-ttu-id="af454-125">Only contacts that are recorded as customers can be assigned a classification based on customer data and only contacts that are recorded as vendors can be assigned a classification based on vendor data.</span><span class="sxs-lookup"><span data-stu-id="af454-125">Only contacts that are recorded as customers can be assigned a classification based on customer data and only contacts that are recorded as vendors can be assigned a classification based on vendor data.</span></span> <span data-ttu-id="af454-126">The automatic classification is not updated automatically.</span><span class="sxs-lookup"><span data-stu-id="af454-126">The automatic classification is not updated automatically.</span></span> <span data-ttu-id="af454-127">Consequently, you may want to update the profile questionnaires, after you have updated the customer, vendor or contact data they are based on.</span><span class="sxs-lookup"><span data-stu-id="af454-127">Consequently, you may want to update the profile questionnaires, after you have updated the customer, vendor or contact data they are based on.</span></span>  

<span data-ttu-id="af454-128">After you have set up automatically answered profile questions, if you assign the profile questionnaire containing these questions to a contact, [!INCLUDE[prod_short](includes/prod_short.md)] will automatically assign the right answers for the contact.</span><span class="sxs-lookup"><span data-stu-id="af454-128">After you have set up automatically answered profile questions, if you assign the profile questionnaire containing these questions to a contact, [!INCLUDE[prod_short](includes/prod_short.md)] will automatically assign the right answers for the contact.</span></span>  

## <a name="example"></a><span data-ttu-id="af454-129">Example</span><span class="sxs-lookup"><span data-stu-id="af454-129">Example</span></span>
<span data-ttu-id="af454-130">You can classify your contacts according to how much they bought from you:</span><span class="sxs-lookup"><span data-stu-id="af454-130">You can classify your contacts according to how much they bought from you:</span></span>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="af454-131"><strong>Answer</strong></span><span class="sxs-lookup"><span data-stu-id="af454-131"><strong>Answer</strong></span></span></th>
<th><span data-ttu-id="af454-132"><strong>Applies to</strong></span><span class="sxs-lookup"><span data-stu-id="af454-132"><strong>Applies to</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="af454-133">A</span><span class="sxs-lookup"><span data-stu-id="af454-133">A</span></span></p></td>
<td><p><span data-ttu-id="af454-134">contacts who bought for 500,000 LCY or more</span><span class="sxs-lookup"><span data-stu-id="af454-134">contacts who bought for 500,000 LCY or more</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="af454-135">B</span><span class="sxs-lookup"><span data-stu-id="af454-135">B</span></span></p></td>
<td><p><span data-ttu-id="af454-136">contacts who bought for 100,000 up to 499,999 LCY</span><span class="sxs-lookup"><span data-stu-id="af454-136">contacts who bought for 100,000 up to 499,999 LCY</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="af454-137">C</span><span class="sxs-lookup"><span data-stu-id="af454-137">C</span></span></p></td>
<td><p><span data-ttu-id="af454-138">contacts who bought for 99,999 LCY or less</span><span class="sxs-lookup"><span data-stu-id="af454-138">contacts who bought for 99,999 LCY or less</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="af454-139">To do this, fill on the **Profile Questionnaire Setup** page as follows:</span><span class="sxs-lookup"><span data-stu-id="af454-139">To do this, fill on the **Profile Questionnaire Setup** page as follows:</span></span>


<table>
<colgroup>
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="af454-140"><strong>Type</strong></span><span class="sxs-lookup"><span data-stu-id="af454-140"><strong>Type</strong></span></span></th>
<th><span data-ttu-id="af454-141"><strong>Description</strong></span><span class="sxs-lookup"><span data-stu-id="af454-141"><strong>Description</strong></span></span></th>
<th><span data-ttu-id="af454-142"><strong>Automatic Classification</strong></span><span class="sxs-lookup"><span data-stu-id="af454-142"><strong>Automatic Classification</strong></span></span></th>
<th><span data-ttu-id="af454-143"><strong>From Value</strong></span><span class="sxs-lookup"><span data-stu-id="af454-143"><strong>From Value</strong></span></span></th>
<th><span data-ttu-id="af454-144"><strong>To Value</strong></span><span class="sxs-lookup"><span data-stu-id="af454-144"><strong>To Value</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="af454-145">Question</span><span class="sxs-lookup"><span data-stu-id="af454-145">Question</span></span></p></td>
<td><p><span data-ttu-id="af454-146">ABC Classification</span><span class="sxs-lookup"><span data-stu-id="af454-146">ABC Classification</span></span></p></td>
<td><p><span data-ttu-id="af454-147">Click to insert a check mark</span><span class="sxs-lookup"><span data-stu-id="af454-147">Click to insert a check mark</span></span></p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="af454-148">Answer</span><span class="sxs-lookup"><span data-stu-id="af454-148">Answer</span></span></p></td>
<td><p><span data-ttu-id="af454-149">A</span><span class="sxs-lookup"><span data-stu-id="af454-149">A</span></span></p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="af454-150">500,000</span><span class="sxs-lookup"><span data-stu-id="af454-150">500,000</span></span></p></td>
<td><p> </p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="af454-151">Answer</span><span class="sxs-lookup"><span data-stu-id="af454-151">Answer</span></span></p></td>
<td><p><span data-ttu-id="af454-152">B</span><span class="sxs-lookup"><span data-stu-id="af454-152">B</span></span></p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="af454-153">100,000</span><span class="sxs-lookup"><span data-stu-id="af454-153">100,000</span></span></p></td>
<td><p><span data-ttu-id="af454-154">499,999</span><span class="sxs-lookup"><span data-stu-id="af454-154">499,999</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="af454-155">Answer</span><span class="sxs-lookup"><span data-stu-id="af454-155">Answer</span></span></p></td>
<td><p><span data-ttu-id="af454-156">C</span><span class="sxs-lookup"><span data-stu-id="af454-156">C</span></span></p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="af454-157">99,999</span><span class="sxs-lookup"><span data-stu-id="af454-157">99,999</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="af454-158">Then fill on the **Profile Question Details** page as follows:</span><span class="sxs-lookup"><span data-stu-id="af454-158">Then fill on the **Profile Question Details** page as follows:</span></span>
<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="af454-159"><strong>Field</strong></span><span class="sxs-lookup"><span data-stu-id="af454-159"><strong>Field</strong></span></span></th>
<th><span data-ttu-id="af454-160"><strong>Value</strong></span><span class="sxs-lookup"><span data-stu-id="af454-160"><strong>Value</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="af454-161"><strong>Customer Classification Field</strong></span><span class="sxs-lookup"><span data-stu-id="af454-161"><strong>Customer Classification Field</strong></span></span></td>
<td><span data-ttu-id="af454-162"><emphasis>Sales (LCY)</emphasis></span><span class="sxs-lookup"><span data-stu-id="af454-162"><emphasis>Sales (LCY)</emphasis></span></span></td>
</tr>
<tr>
<td><span data-ttu-id="af454-163"><strong>Classification Method</strong></span><span class="sxs-lookup"><span data-stu-id="af454-163"><strong>Classification Method</strong></span></span></td>
<td><span data-ttu-id="af454-164"><emphasis>Defined Value</emphasis></span><span class="sxs-lookup"><span data-stu-id="af454-164"><emphasis>Defined Value</emphasis></span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="af454-165">When you assign the profile questionnaire containing this question to a contact, application automatically enters the relevant answer for this contact on the profile lines of the contact card.</span><span class="sxs-lookup"><span data-stu-id="af454-165">When you assign the profile questionnaire containing this question to a contact, application automatically enters the relevant answer for this contact on the profile lines of the contact card.</span></span>

## <a name="see-also"></a><span data-ttu-id="af454-166">See Also</span><span class="sxs-lookup"><span data-stu-id="af454-166">See Also</span></span>
[<span data-ttu-id="af454-167">Creating Contacts</span><span class="sxs-lookup"><span data-stu-id="af454-167">Creating Contacts</span></span>](marketing-create-contact-companies.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]