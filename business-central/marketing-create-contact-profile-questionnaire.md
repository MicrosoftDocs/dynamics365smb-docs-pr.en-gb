---
title: Use profiles to classify contacts
description: Set up profile questionnaires to help classify your business contacts
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: contacts, profiles
ms.author: edupont
ms.date: 04/01/2019
ms.openlocfilehash: fe02153a89ad5f63855cff5eec5344d601c8663a
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: en-GB
ms.lasthandoff: 03/31/2019
ms.locfileid: "934449"
---
# <a name="use-profile-questionnaires-to-classify-business-contacts"></a><span data-ttu-id="bc576-103">Use Profile Questionnaires to Classify Business Contacts</span><span class="sxs-lookup"><span data-stu-id="bc576-103">Use Profile Questionnaires to Classify Business Contacts</span></span>
<span data-ttu-id="bc576-104">You can set up profile questionnaires that you want to use when entering information about your contacts' profiles.</span><span class="sxs-lookup"><span data-stu-id="bc576-104">You can set up profile questionnaires that you want to use when entering information about your contacts' profiles.</span></span> <span data-ttu-id="bc576-105">Within each questionnaire, you can set up the different questions you intend to ask your contacts.</span><span class="sxs-lookup"><span data-stu-id="bc576-105">Within each questionnaire, you can set up the different questions you intend to ask your contacts.</span></span>  

<span data-ttu-id="bc576-106">You can also run the questionnaire to answer some of the questions based on contact, customer, or vendor data automatically.</span><span class="sxs-lookup"><span data-stu-id="bc576-106">You can also run the questionnaire to answer some of the questions based on contact, customer, or vendor data automatically.</span></span>  

## <a name="to-add-a-profile-questionnaire"></a><span data-ttu-id="bc576-107">To add a profile questionnaire</span><span class="sxs-lookup"><span data-stu-id="bc576-107">To add a profile questionnaire</span></span>
1.  <span data-ttu-id="bc576-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Questionnaire Setup**, and then choose the related link.</span><span class="sxs-lookup"><span data-stu-id="bc576-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Questionnaire Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="bc576-109">On the **Home** tab, in the **New** group, choose **New**.</span><span class="sxs-lookup"><span data-stu-id="bc576-109">On the **Home** tab, in the **New** group, choose **New**.</span></span>  
3.  <span data-ttu-id="bc576-110">Fill in the fields as necessary.</span><span class="sxs-lookup"><span data-stu-id="bc576-110">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-add-questions-to-a-profile-questionnaire"></a><span data-ttu-id="bc576-111">To add questions to a profile questionnaire</span><span class="sxs-lookup"><span data-stu-id="bc576-111">To add questions to a profile questionnaire</span></span>
1.  <span data-ttu-id="bc576-112">Choose the relevant profile questionnaire, and then on the **Home** tab, in the **Process** group, choose **Edit Questionnaire Setup**.</span><span class="sxs-lookup"><span data-stu-id="bc576-112">Choose the relevant profile questionnaire, and then on the **Home** tab, in the **Process** group, choose **Edit Questionnaire Setup**.</span></span>  
2.  <span data-ttu-id="bc576-113">On the first empty line, in the **Type** field, choose **Question** and type your question in the **Description** field.</span><span class="sxs-lookup"><span data-stu-id="bc576-113">On the first empty line, in the **Type** field, choose **Question** and type your question in the **Description** field.</span></span> <span data-ttu-id="bc576-114">Fill in the other fields on this line.</span><span class="sxs-lookup"><span data-stu-id="bc576-114">Fill in the other fields on this line.</span></span>  
3.  <span data-ttu-id="bc576-115">On the next empty line, in the **Type** field, choose **Answer** and type your answer in the **Description** field.</span><span class="sxs-lookup"><span data-stu-id="bc576-115">On the next empty line, in the **Type** field, choose **Answer** and type your answer in the **Description** field.</span></span>  
4.  <span data-ttu-id="bc576-116">In the **Priority** field, select the priority.</span><span class="sxs-lookup"><span data-stu-id="bc576-116">In the **Priority** field, select the priority.</span></span> <span data-ttu-id="bc576-117">In the **From Value** and **To Value** fields, define a point range.</span><span class="sxs-lookup"><span data-stu-id="bc576-117">In the **From Value** and **To Value** fields, define a point range.</span></span> <span data-ttu-id="bc576-118">Contacts that receive points within the defined range will get the answer.</span><span class="sxs-lookup"><span data-stu-id="bc576-118">Contacts that receive points within the defined range will get the answer.</span></span>  

<span data-ttu-id="bc576-119">Repeat these steps to enter all the questions and answers within the profile questionnaire.</span><span class="sxs-lookup"><span data-stu-id="bc576-119">Repeat these steps to enter all the questions and answers within the profile questionnaire.</span></span>

<span data-ttu-id="bc576-120">After you have created a questionnaire, you must create contact ratings to classify your contacts.</span><span class="sxs-lookup"><span data-stu-id="bc576-120">After you have created a questionnaire, you must create contact ratings to classify your contacts.</span></span> <span data-ttu-id="bc576-121">You can also set up questions that are rated automatically based on information in the contact card.</span><span class="sxs-lookup"><span data-stu-id="bc576-121">You can also set up questions that are rated automatically based on information in the contact card.</span></span>  

> [!NOTE]
> <span data-ttu-id="bc576-122">If you enter a question that is automatically answered, choose <STRONG>Line</STRONG>, and then choose <STRONG>Question Details</STRONG>, to enter the criteria to automatically answer the question.</span><span class="sxs-lookup"><span data-stu-id="bc576-122">If you enter a question that is automatically answered, choose <STRONG>Line</STRONG>, and then choose <STRONG>Question Details</STRONG>, to enter the criteria to automatically answer the question.</span></span>

## <a name="the-automatic-classification-of-contacts"></a><span data-ttu-id="bc576-123">The Automatic Classification of Contacts</span><span class="sxs-lookup"><span data-stu-id="bc576-123">The Automatic Classification of Contacts</span></span>
<span data-ttu-id="bc576-124">You can automatically classify your contacts according to customer, vendor, and contact information, by setting up automatically answered profile questions on the **Profile Questionnaire Setup** page.</span><span class="sxs-lookup"><span data-stu-id="bc576-124">You can automatically classify your contacts according to customer, vendor, and contact information, by setting up automatically answered profile questions on the **Profile Questionnaire Setup** page.</span></span>  

> [!NOTE]
> <span data-ttu-id="bc576-125">Only contacts that are recorded as customers can be assigned a classification based on customer data and only contacts that are recorded as vendors can be assigned a classification based on vendor data.</span><span class="sxs-lookup"><span data-stu-id="bc576-125">Only contacts that are recorded as customers can be assigned a classification based on customer data and only contacts that are recorded as vendors can be assigned a classification based on vendor data.</span></span> <span data-ttu-id="bc576-126">The automatic classification is not updated automatically.</span><span class="sxs-lookup"><span data-stu-id="bc576-126">The automatic classification is not updated automatically.</span></span> <span data-ttu-id="bc576-127">Consequently, you may want to update the profile questionnaires, after you have updated the customer, vendor or contact data they are based on.</span><span class="sxs-lookup"><span data-stu-id="bc576-127">Consequently, you may want to update the profile questionnaires, after you have updated the customer, vendor or contact data they are based on.</span></span>  

<span data-ttu-id="bc576-128">After you have set up automatically answered profile questions, if you assign the profile questionnaire containing these questions to a contact, [!INCLUDE[d365fin](includes/d365fin_md.md)] will automatically assign the right answers for the contact.</span><span class="sxs-lookup"><span data-stu-id="bc576-128">After you have set up automatically answered profile questions, if you assign the profile questionnaire containing these questions to a contact, [!INCLUDE[d365fin](includes/d365fin_md.md)] will automatically assign the right answers for the contact.</span></span>  

## <a name="example"></a><span data-ttu-id="bc576-129">Example</span><span class="sxs-lookup"><span data-stu-id="bc576-129">Example</span></span>
<span data-ttu-id="bc576-130">You can classify your contacts according to how much they bought from you:</span><span class="sxs-lookup"><span data-stu-id="bc576-130">You can classify your contacts according to how much they bought from you:</span></span>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="bc576-131"><strong>Answer</strong></span><span class="sxs-lookup"><span data-stu-id="bc576-131"><strong>Answer</strong></span></span></th>
<th><span data-ttu-id="bc576-132"><strong>Applies to</strong></span><span class="sxs-lookup"><span data-stu-id="bc576-132"><strong>Applies to</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="bc576-133">A</span><span class="sxs-lookup"><span data-stu-id="bc576-133">A</span></span></p></td>
<td><p><span data-ttu-id="bc576-134">contacts who bought for 500,000 LCY or more</span><span class="sxs-lookup"><span data-stu-id="bc576-134">contacts who bought for 500,000 LCY or more</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="bc576-135">B</span><span class="sxs-lookup"><span data-stu-id="bc576-135">B</span></span></p></td>
<td><p><span data-ttu-id="bc576-136">contacts who bought for 100,000 up to 499,999 LCY</span><span class="sxs-lookup"><span data-stu-id="bc576-136">contacts who bought for 100,000 up to 499,999 LCY</span></span></p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="bc576-137">C</span><span class="sxs-lookup"><span data-stu-id="bc576-137">C</span></span></p></td>
<td><p><span data-ttu-id="bc576-138">contacts who bought for 99,999 LCY or less</span><span class="sxs-lookup"><span data-stu-id="bc576-138">contacts who bought for 99,999 LCY or less</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="bc576-139">To do this, fill on the **Profile Questionnaire Setup** page as follows:</span><span class="sxs-lookup"><span data-stu-id="bc576-139">To do this, fill on the **Profile Questionnaire Setup** page as follows:</span></span>


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
<th><span data-ttu-id="bc576-140"><strong>Type</strong></span><span class="sxs-lookup"><span data-stu-id="bc576-140"><strong>Type</strong></span></span></th>
<th><span data-ttu-id="bc576-141"><strong>Description</strong></span><span class="sxs-lookup"><span data-stu-id="bc576-141"><strong>Description</strong></span></span></th>
<th><span data-ttu-id="bc576-142"><strong>Automatic Classification</strong></span><span class="sxs-lookup"><span data-stu-id="bc576-142"><strong>Automatic Classification</strong></span></span></th>
<th><span data-ttu-id="bc576-143"><strong>From Value</strong></span><span class="sxs-lookup"><span data-stu-id="bc576-143"><strong>From Value</strong></span></span></th>
<th><span data-ttu-id="bc576-144"><strong>To Value</strong></span><span class="sxs-lookup"><span data-stu-id="bc576-144"><strong>To Value</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><span data-ttu-id="bc576-145">Question</span><span class="sxs-lookup"><span data-stu-id="bc576-145">Question</span></span></p></td>
<td><p><span data-ttu-id="bc576-146">ABC Classification</span><span class="sxs-lookup"><span data-stu-id="bc576-146">ABC Classification</span></span></p></td>
<td><p><span data-ttu-id="bc576-147">Click to insert a check mark</span><span class="sxs-lookup"><span data-stu-id="bc576-147">Click to insert a check mark</span></span></p></td>
<td><p> </p></td>
<td><p> </p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="bc576-148">Answer</span><span class="sxs-lookup"><span data-stu-id="bc576-148">Answer</span></span></p></td>
<td><p><span data-ttu-id="bc576-149">A</span><span class="sxs-lookup"><span data-stu-id="bc576-149">A</span></span></p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="bc576-150">500,000</span><span class="sxs-lookup"><span data-stu-id="bc576-150">500,000</span></span></p></td>
<td><p> </p></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="bc576-151">Answer</span><span class="sxs-lookup"><span data-stu-id="bc576-151">Answer</span></span></p></td>
<td><p><span data-ttu-id="bc576-152">B</span><span class="sxs-lookup"><span data-stu-id="bc576-152">B</span></span></p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="bc576-153">100,000</span><span class="sxs-lookup"><span data-stu-id="bc576-153">100,000</span></span></p></td>
<td><p><span data-ttu-id="bc576-154">499,999</span><span class="sxs-lookup"><span data-stu-id="bc576-154">499,999</span></span></p></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="bc576-155">Answer</span><span class="sxs-lookup"><span data-stu-id="bc576-155">Answer</span></span></p></td>
<td><p><span data-ttu-id="bc576-156">C</span><span class="sxs-lookup"><span data-stu-id="bc576-156">C</span></span></p></td>
<td><p> </p></td>
<td><p> </p></td>
<td><p><span data-ttu-id="bc576-157">99,999</span><span class="sxs-lookup"><span data-stu-id="bc576-157">99,999</span></span></p></td>
</tr>
</tbody>
</table>

<span data-ttu-id="bc576-158">Then fill on the **Profile Question Details** page as follows:</span><span class="sxs-lookup"><span data-stu-id="bc576-158">Then fill on the **Profile Question Details** page as follows:</span></span>
<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="bc576-159"><strong>Field</strong></span><span class="sxs-lookup"><span data-stu-id="bc576-159"><strong>Field</strong></span></span></th>
<th><span data-ttu-id="bc576-160"><strong>Value</strong></span><span class="sxs-lookup"><span data-stu-id="bc576-160"><strong>Value</strong></span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="bc576-161"><strong>Customer Classification Field</strong></span><span class="sxs-lookup"><span data-stu-id="bc576-161"><strong>Customer Classification Field</strong></span></span></td>
<td><span data-ttu-id="bc576-162"><emphasis>Sales (LCY)</emphasis></span><span class="sxs-lookup"><span data-stu-id="bc576-162"><emphasis>Sales (LCY)</emphasis></span></span></td>
</tr>
<tr>
<td><span data-ttu-id="bc576-163"><strong>Classification Method</strong></span><span class="sxs-lookup"><span data-stu-id="bc576-163"><strong>Classification Method</strong></span></span></td>
<td><span data-ttu-id="bc576-164"><emphasis>Defined Value</emphasis></span><span class="sxs-lookup"><span data-stu-id="bc576-164"><emphasis>Defined Value</emphasis></span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="bc576-165">When you assign the profile questionnaire containing this question to a contact, the programme automatically enters the relevant answer for this contact on the profile lines of the contact card.</span><span class="sxs-lookup"><span data-stu-id="bc576-165">When you assign the profile questionnaire containing this question to a contact, the program automatically enters the relevant answer for this contact on the profile lines of the contact card.</span></span>

## <a name="see-also"></a><span data-ttu-id="bc576-166">See Also</span><span class="sxs-lookup"><span data-stu-id="bc576-166">See Also</span></span>
[<span data-ttu-id="bc576-167">Creating Contacts</span><span class="sxs-lookup"><span data-stu-id="bc576-167">Creating Contacts</span></span>](marketing-create-contact-companies.md)  
